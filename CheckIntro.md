### Check:
  <p>Unit testing in C is generally harder than other than other languages.
  In other languages, the worst scenario is that the unit test fails throwing an exception. 
  In C, in addition to this, the address space can be trashed. 
  If the test framework resides in the same location, then we will lose the framework.
  Check uses the fork() system call to create a new address space. Each unit test is run in this space. Message queues to send information on the testing process back to the test framework. 
  Thus, we can effectively manage issues caused by pointers, segmentation faults etc. and continue testing. </p>
