
- Let us see a case where the test can fail. 
- In the arithmetic.java file, we shall change the sum function.

>import java.util.*;<br>
><br>
>public class arithmetic<br>
>{<br>
>public int arithmeticmethod()<br>
>{<br>
>int sum =0,i; <br>
>for(i=1;i<=10;i++)<br>
>{<br>
>sum -= i;   ----------------------- This statement was changed<br>
>}<br>
>return sum;<br>
><br>
>}<br>
>public static void main(String args[])<br>
>{<br>
>}<br>
>}<br>

- Now, when we test the file, since the actual outcome does not match the expected outcome, the test fails and the output is shown as below.
