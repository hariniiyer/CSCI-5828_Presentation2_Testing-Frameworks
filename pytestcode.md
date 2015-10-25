

Here is an example for PyTest. It is basic test to see if a function works according to the command line argument given.

<code><pre>
def test_answer(cmdopt):
    if cmdopt == "type1":
        print ("first")
    elif cmdopt == "type2":
        print ("second")
    assert 0 # to see what was printed
</pre></code>

[NEXT](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/nose.md)

[BACK](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/pytest.md)
