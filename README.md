What is Interpreter Pattern?

    Interpreter pattern is used to define a grammatical representation for a language and provides an interpreter to deal with this grammar.

Components

    1. Expression

    2. IntToBinaryExpression

    3. IntToHexExpression

    4. IntepreterContext

    5. InterpreterClient

1. Expression

   has the 'interpret' method with the InterpreterContext ic.

2) IntToBinaryExpression

   Impelements 'Expression' Interface
   This sets the Integer

   Overrides the 'interpret' method based on the context passed

3. IntToHexExpression

   Impelements 'Expression' Interface
   This sets the Integer

   Overrides the 'interpret' method based on the context passed

4)  IntepreterContext

    holds the methods of the 2 expression which they will call when they override the method 'interpret' located in 'Expression' Interface

5. InterpreterClient

   Instantiate an Object of its class with an InterpreterContext executing both Interpreters which implement the 'Expression' Interface
