### Check:
  <p>Unit testing in C is generally harder than other languages
  since there is a possibility of the address space being trashed. 
  If the test framework resides in the same location, then we will lose the framework.
  Check uses the fork() system call to create a new address space. Each unit test is run in this space. Message queues to send information on the testing process back to the test framework. 
  Thus, we can effectively manage memory location issues caused by pointers, segmentation faults etc. and continue testing. </p>

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CUnitExample.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CheckFeatures.md)
