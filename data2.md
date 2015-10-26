
<b>TESTING:</b>

<code><pre>
@RunWith(JUnitParamsRunner.class)<br>
public class FullHouseTest <br>
{<br>

@Test<br>
@Parameters<br>
public void fullHouse(Collection rolled, int score)<br> 
{<br>
assertThat(new FullHouse().getScore(rolled).getValue()).isEqualTo(score);<br>
}<br>
<br>
public Object[] parametersForFullHouse()<br> 
{<br>
return $(<br>
$(roll(1, 1, 1, 2, 2), score(7)),<br>
$(roll(1, 1, 2, 2, 2), score(8)),<br>
$(roll(5, 5, 5, 2, 2), score(19)),<br>
);<br>
}<br>
<br>
private static int score(int score) <br>
{<br>
return score;<br>
}<br>
}<br>


Thus we are able to add different test data sets and run them with ease without having the need to modify the given test data set each and every time.

<br>

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/data1.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/data3.md)

