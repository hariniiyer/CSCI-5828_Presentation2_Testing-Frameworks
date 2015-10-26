### Mocking in NovaProva:
   A problem in testing is the interdependence of modules. To solve this problem, NovaProva uses a concept
   called mocking. Mocking is a technique by which modules that don't needed to be tested are replaced with <I>mock</I> versions
   that have simpler and more controllable behavior. When NovaProva finds a function whose name starts with the letters <I>mock_</I>, 
   it automatically adds that function as a mock to all the tests defined in the same source file. Mocks are automatically installed 
   and uninstalled when the tests start and end respectively. Additionally, NovaProva allows dynamic mocks that allow mocks
   to ba added and removed partway through a test. 
For example, consider a module foo.
<pre><code>void foo_mustache(int x)
{
    BarTxn *txn = bar_begin();
    int r = bar_shoreditch(x);
    if (r < 0)
    {
        fprintf(stderr, "shoreditch failed: %d", -r);
        return;
    }
    bar_commit(txn);
}</pre></code>

<I>bar_shoreditch()</I> returns an error when an earlier call to <I>bar_begin()</I> leaked <I>BarTxn</I>. 
Hence,we mock <I>bar_shoreditch()</I> as follows:
<pre><code>int mock_bar_shoreditch(int x)
{
    if (x == 42)
        return -ENOENT;
    return 0;
}</pre></code>
   
Now, dynamic mocking can be acheived as follows:   
   <pre><code> static int fail_with_enoent(int x)
{
    return -ENOENT;
}

void test_some_ditches(void)
{
    foo_mustache(0);    // calls the real bar_shoreditch() 
    foo_mustache(1);
    np_mock(bar_shoreditch, fail_with_enoent);
    foo_mustache(2);    // calls the mock
    np_unmock(bar_shoreditch);
    foo_mustache(3);    // calls the real bar_shoreditch() again 
}
</pre></code>



[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/NovaProvaDesign.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/NovaProvaExample.md)
