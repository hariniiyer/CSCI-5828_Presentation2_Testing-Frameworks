### Mocking:
   A problem in testing is the interdependence of modules. To solve this problem, NovaProva uses a concept
   called mocking. Mocking is a technique by which modules that don't needed to be tested are replaced with <I>mock</I> versions
   that have simpler and more controllable behavior. When NovaProva finds a function whose name starts with the letters <I>mock_</I>, 
   it automatically adds that function as a mock to all the tests defined in the same source file. Mocks are automatically installed 
   and uninstalled when the tests start and end respectively.
