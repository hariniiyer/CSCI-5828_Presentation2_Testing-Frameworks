### Unit Testing in C:
   C is an imperative language designed to be compiled using a relatively straightforward compiler. It provides low-level access to memory and language constructs that map efficiently to machine instructions. It requires minimal run-time support. Unit testing in C is similar in several aspects to unit testing in Python, Java etc. However, there are
   certain addtional issues.  In other languages, the worst scenario is that the unit test fails and throws an exception.
   However, in C, there is an additional problem of the address space being trashed. If important information resides 
   in these locations, then the complications are amplified. Hence, additional care should be taken in modelling testing
   frameworks for C. Here, we overview three testing frameworks for C.
   1. <b>CUnit</b>
   2. <b>Check</b>
   3. <b>NovaProva</b>
   
   



[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/hybrid14.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" 
height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CUnit.md)
