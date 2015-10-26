### Example:
   The following is a test case to validate the class <I>money</I>
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

[<img src="https://cloud.githubusercontent.com/assets/14101008/10718970/e8253ecc-7b43-11e5-8fcb-af3acab64686.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/CheckSyntax.md)
[<img src="https://cloud.githubusercontent.com/assets/14101008/10718969/e5b6db32-7b43-11e5-886a-b848ca79f105.png" width="50" height="50"></img>](https://github.com/hariniiyer/CSCI-5828_Presentation2_Testing-Frameworks/blob/master/NovaProvaIntro.md)
