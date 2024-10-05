Strategy Design Pattern Example
This repository demonstrates the Strategy Design Pattern in Java. The Strategy Pattern defines a family of algorithms, encapsulates each one, and makes them interchangeable. The pattern allows the algorithm to vary independently from the clients that use it.

Overview
The main class Main demonstrates the use of the Strategy Design Pattern. The pattern is implemented by defining a Strategy interface with multiple concrete strategy classes (OperationAdd, OperationSubtract, OperationMultiply). A Context class is used to execute the chosen strategy.

Classes
Strategy (Interface):

Declares the method doOperation(int num1, int num2), which is implemented by concrete strategy classes.
OperationAdd:

Implements the Strategy interface to perform addition.
OperationSubtract:

Implements the Strategy interface to perform subtraction.
OperationMultiply:

Implements the Strategy interface to perform multiplication.
Context:

Holds a reference to a Strategy object and provides a method executeStrategy to execute the selected strategy.
Main:

Demonstrates the use of different strategies (addition, subtraction, multiplication) through the Context class.
Main Class: Main
The Main class contains the main method, which demonstrates the following:

Creating a Context object with an OperationAdd strategy and using it to add two numbers.
Changing the strategy to OperationSubtract to subtract two numbers.
Finally, switching the strategy to OperationMultiply to multiply two numbers.
