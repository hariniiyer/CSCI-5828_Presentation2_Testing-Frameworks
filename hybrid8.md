- Let arithmetictest.java be the testing file created in java.

- We need to import org.junit.Test and org.junit.Assert.* packages for the file that is going to perform the test.

- @Test is the annotation used inorder to make the system understand that it is the test that has to be run.

<code><pre>
//Arithmetictest.java

import java.util.*;<br>  
import static org.junit.Assert.assertEquals;<br>
import org.junit.Test;<br>
<br>
public class arithmetictest<br>
{<br>
@Test<br>
public void evaluate()<br>
{<br>
arithmetic a= new arithmetic();<br>
int sum=a.arithmeticmethod();	<br>
assertEquals(55,sum);<br>
}<br>
<br>
public static void main(String args[])<br>
{}<br>
}<br>
</pre></code>
<br>

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/hybrid7.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/hybrid9.md)
