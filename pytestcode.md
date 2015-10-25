

Following is a basic example of unnittest. 

The test method is class SimplisticTest would fail if the passes parameter becomes false. 


<pre><code>
import unittest

class SimplisticTest(unittest.TestCase):

    def test(self):
        self.failUnless(True)

if __name__ == '__main__':
    unittest.main()
    
</code></pre>
