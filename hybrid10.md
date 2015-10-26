
- Let us see a case where the test can fail. 
- In the arithmetic.java file, we shall change the sum function.
<code><pre>
import java.util.*;<br>
<br>
public class arithmetic<br>
{<br>
public int arithmeticmethod()<br>
{<br>
int sum =0,i; <br>
for(i=1;i<=10;i++)<br>
{<br>
sum -= i;   ----------------------- This statement was changed<br>
}<br>
return sum;<br>
<br>
}<br>
public static void main(String args[])<br>
{<br>
}<br>
}<br>
</pre></code>
- Now, when we test the file, since the actual outcome does not match the expected outcome, the test fails and the output is shown as below.

<br>

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/hybrid9.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/hybrid11.md)

