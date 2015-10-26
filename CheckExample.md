### Example:
   The following is a test case to validate the class <I>money</I>. This class is from a library used to handle currency.

<pre><code>
\#include "check.h"
\#include "../src/money.h"
   
START_TEST(test_money_create)
{
  Money *m;
  m = money_create(5, "USD");
  ck_assert_int_eq(money_amount(m), 5);
  ck_assert_str_eq(money_currency(m), "USD");
  money_free(m);
}
END_TEST
   
int main(void)
{
  return 0;
}
</pre></code>

A unit test should execute and finish. If it exits early or is signaled, it will fail with an error message. Special calls
are required to determine the exact nature of the failure. Hence, we use:
<p>1. <I>ck_assert_int_eq</I> (to determine if two integers are equal) </p>
<p>2. <I>ck_assert_str_eq</I> (to determine if two null terminated strings are equal). </p>
Both macros will signal an error if their arguments are not equal.

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CheckSyntax.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/NovaProvaIntro.md)
