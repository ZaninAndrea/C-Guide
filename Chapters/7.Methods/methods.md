# Methods
## THEORY
Methods are a handy way to reuse the same piece of code, in the most basic form a method once invoked (we’ll come back to this later) executes a piece of code. More advanced types of methods allow the method to return a value (you can use the method interchangeably with the value it returns, just like variables). A method can also require some inputs.  
## PRACTICE  
The syntax to declare a method is  
```
typeReturned methodName (inputs declarations){
	//code
	return valueToReturn;
}
```  
Let’s dig into this syntax:
- *typeReturned* is the type of the value to return, could be `float`, `string`, `int`,… If your method doesn’t return any value use the type `void`
- *methodName* is the name that you will use to invoke the method, similar to a variable’s name
- *input declarations* are the declaration of the input, separated by commas e.g. `int x, int y` if you need no input leave it void
- the code inside the curly brackets will be executed once the method is invoked
- lastly we have the `return` keyword, you can use the syntax `return value` to return a value (similarly to assigning a value to a variable). After calling `return` the method will stop executing

> ::exlamation-triangle:: DON'T FORGET  
> The pair *methodName* and *input delcaration* has to be unique inside the cope of the function (at the moment you can ignore the *scope-part* of the sentence)  

The variables declared as input don't need to be assigned before being used, because you will asign them a value when you invoke the method.  
Speaking of invoking here is the syntax:  
`methodName(input values)`  
The input values must be separated by commas, if the method requires no input just leave it void (literally void, not `void` the type).  

## Examples
A method that takes a number and returns it plus 2:  
```
// method declaration
int addTwo (int x){
	y=x+2;
	return y;
}
//using the method
int y=3;
y=addTwo(y); //y now has a value of 5
```  
As you can see I used a variable as input when invoking the function and this is perfectly fine.  

## ADVANCED
Remember the starting code that visual studio provided you? If you look carefully, you’ll see that there’s the declaration for the Main method. The Main method is automatically executed once you start the program  

## ASSIGNEMENT
Write a program that has a method that takes as input a string and returns the string doubled e.g. input: <kbd>hello</kbd>, output: <kbd>hellohello</kbd>. Then take an input from the console and use the method to double it, write on the console the result.  
TIPS:  
- remember that you can concatenate strings using the `+` sign  

SOLUTION:  
```
//declaring the method
string doubleIt(string input){
	return input+input; //returning the string doubled
}
string a= Console.ReadLine();
Console.WriteLine( doubleIt(a) );
//I used the method doubleIt as input for the WriteLine method
```

