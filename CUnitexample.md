### Example:
  The syntax for a CUnit test is :  
  <pre><code>void test_function(void)</code></pre>
  
  Consider a function that returns the maximum of two integers:
  <pre><code> int maxi(int i1, int i2)
    {
      return (i1 > i2) ? i1 : i2;
    }
 </code></pre>
    
 The test function will be as follows:
    
    <pre><code>  void test_maxi(void)
    {
      CU_ASSERT(maxi(0,2) == 2);
      CU_ASSERT(maxi(0,-2) == 0);
      CU_ASSERT(maxi(2,2) == 2);
    } 
</code></pre>


[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CUnitA&R.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CheckIntro.md)
