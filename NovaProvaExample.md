###Example: 
  Consider a test function that tests the funcionality of <I>myatoi</I>. <I>myatoi</I> takes in a 
  string and converts it to an integer.
<pre><code>
\#include "mycode.h"
int myatoi(const char *s)
{
    int v = 0;
    for ( ; *s ; s++)
    {
        v *= 10;
        v += (*s - '0');
    }
    return v;
}
</pre></code>

The test is as follows:
<pre><code>
/* mytest.c */
\#include "np.h"         /* NovaProva library */
\#include "mycode.h"     /* declares the Code Under Test */
static void test_simple(void)
{
    int r;
    r = myatoi("42");
    NP_ASSERT_EQUAL(r, 42);
}
</pre></code>
