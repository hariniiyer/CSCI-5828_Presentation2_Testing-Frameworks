
####UNITTEST

VEry very very import : cpuy

http://www.drdobbs.com/testing/unit-testing-with-python/240165163

![unittest module](http://twimgs.com/ddj/images/article/2014/0114/PythonUnitTest1.gi)

import unittest
from unnecessary_math import multiply
 
class TestUM(unittest.TestCase):
 
    def test_numbers_3_4(self):
        self.assertEqual( multiply(3,4), 12)
 
 
 
