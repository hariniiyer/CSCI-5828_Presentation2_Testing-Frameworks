<b>EXAMPLE CODE:</b>

<p>In this example,we calculate the score of the fullhouse(fullhouse will have 3 numbers of one kind and 2 numbers of another kind) and we assume the score to be the sum of all numbers in a roll.
</p>

>class FullHouse implements Scoreable<br> 
>{<br>
>public Score getScore(Collection dice) <br>
>{<br>
>Score pairScore = Scorables.pair().getScore(dice);<br>
>Score threeOfAKindScore = Scorables.threeOfAKind().getScore.(pairScore.getReminder());<br>
>        
>if (bothAreGreaterThanZero(pairScore.getValue(), threeOfAKindScore.getValue()))<br> 
>{<br>
>            return new Score(pairScore.getValue() + threeOfAKindScore.getValue()); // no reminder<br>
>}<br>
>return new Score(0, dice);<br>
>}<br>
><br>
>private boolean bothAreGreaterThanZero(int value1, int value2)<br> 
>{<br>
>return value1 > 0 && value2 > 0;<br>
>}<br>
>}<br>
<br>

Some of the unit tests if we wish to do are:

- Score is 7 for the numbers: 1 1 1 2 2
- Score is 8 for the numbers: 1 1 2 2 2
- Score is 19 for the numbers: 5 5 5 2 2
