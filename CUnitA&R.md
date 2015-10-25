### Assertions:
   CUnit provides a set of assertions for testing logical conditions.
   Each assertion tests a single logical condition, and fails if the condition evaluates to FALSE.
   
### Running tests:
  CUnit supports running all tests in all registered suites, but individual tests or suites can also be run. 
  During each run, the framework keeps track of the number of suites, tests, and assertions run, passed, and failed.
  The interfaces included in the CUnit library are:
  1. <b>Automated</b> - non-interactive and outputs to XML file
  2. <b>Basic</b>     - non-interactive and optional output to stdout
  3. <b>Console</b>   - interactive control mode under user control
  4. <b>Curses</b>    - interactive curses mode under user control
