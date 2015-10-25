

VEry very very import : cpuy

http://www.drdobbs.com/testing/unit-testing-with-python/240165163



import unittest
from unnecessary_math import multiply
 
class TestUM(unittest.TestCase):
 
    def test_numbers_3_4(self):
        self.assertEqual( multiply(3,4), 12)
 
 
 
