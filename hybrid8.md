- Let arithmetictest.java be the testing file created in java.

- We need to import org.junit.Test and org.junit.Assert.* packages for the file that is going to perform the test.

- @Test is the annotation used inorder to make the system understand that it is the test that has to be run.

//Arithmetictest.java

>import java.util.*;<br>  
>import static org.junit.Assert.assertEquals;<br>
>import org.junit.Test;<br>
><br>
>public class arithmetictest<br>
>{<br>
>@Test<br>
>public void evaluate()<br>
>{<br>
>arithmetic a= new arithmetic();<br>
>int sum=a.arithmeticmethod();	<br>
>assertEquals(55,sum);<br>
>}<br>
><br>
>public static void main(String args[])<br>
>{}<br>
>}<br>
