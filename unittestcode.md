

Following is a basic example of unnittest. 

The test method in class SimplisticTest would fail if the passes parameter becomes false. 


<pre><code>
import unittest

class SimplisticTest(unittest.TestCase):

    def test(self):
        self.failUnless(True)

if __name__ == '__main__':
    unittest.main()
    
</code></pre>


[NEXT](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/nose.md)

[BACK](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/unittest.md)
