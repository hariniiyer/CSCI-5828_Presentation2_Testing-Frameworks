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
