
<b>TESTING:</b>

>@RunWith(JUnitParamsRunner.class)<br>
>public class FullHouseTest <br>
>{<br>
>
>@Test<br>
>@Parameters<br>
>public void fullHouse(Collection rolled, int score)<br> 
>{<br>
>assertThat(new FullHouse().getScore(rolled).getValue()).isEqualTo(score);<br>
>}<br>
><br>
>public Object[] parametersForFullHouse()<br> 
>{<br>
>return $(<br>
>$(roll(1, 1, 1, 2, 2), score(7)),<br>
>$(roll(1, 1, 2, 2, 2), score(8)),<br>
>$(roll(5, 5, 5, 2, 2), score(19)),<br>
>);<br>
>}<br>
><br>
>private static int score(int score) <br>
>{<br>
>return score;<br>
>}<br>
>}<br>


Thus we are able to add different test data sets and run them with ease without having the need to modify the given test data set each and every time.
