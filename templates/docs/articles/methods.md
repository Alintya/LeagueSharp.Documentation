Methods
===================

Introduction
-------------
A method is a collection of several operations grouped together in order to perform a task.

There is one method you already know, the Main method every program has.

Methods must be defined before they can be used (=called).


Defining a Method
-------------

Method definitions follow a strict syntax:

    <Access Specifier> <Return Type> <Method Name>(Parameter List)
	{
	   //Method Body
	}

Let's look at the definition of our previous "Main" method

    static void Main(string[] args)
    {
    }

To split things up;

>  Access Modifier = static
>  Return Type = void
>  Method Name = Main
> Parameter List = A single parameter of type string[], named "args" 

The [access modifier](access_modifiers.md) defines who can access this method and from where in your code it is allowed to do so.

The return type determines whether this method is supposed to return something to it's caller and more ultimately, which type of information/variable -> [Variables](variables.md)    
In our case, the return type is void, meaning this function has no returning value.

A method's parameters are variables passed to it by it's caller.The method can work with them and/or modifiy their content.
You can define as many parameters as you wish. Every parameter is given a type and a name, just as you do with methods.
One thing to care about are reference types;

You can pass variables by value, as well as by reference.

| Type |         Description        |
|:------------:|:--------------------------:|
|     [Value parameters](value_parameters.md)    | This method copies the actual value of an argument into the formal parameter of the function. In this case, changes made to the parameter inside the function have no effect on the argument.|
|    [Reference parameters](reference_parameters.md)   |      This method copies the reference to the memory location of an argument into the formal parameter. This means that changes made to the parameter affect the argument.|
|      [Output parameters](output_parameters.md)     |      This method helps in returning more than one value.|


Calling a Method
-------------

A method is called by simply using it's name followed by brackets and the usual semicolon;

    myfuntion();
    
----------------
**Example program:**

        class Program
    {
        static void Main(string[] args)
        {
	        int number1 = 10;
	        int number2 = 20;
	        
	        System.Console.WriteLine(Sum(number1, number2));
        }
        static int Sum(int a, int b)
        {
	        return(a + b);
        }
    }


> Expected output: 30

This example featured everything we discussed until now.
It declares 2 variables, "number1" and "number2" and assigns values to them.
the method "WriteLine" of namespace "System.Console" is called with the return value of our "Sum" funtion defined below, which is given 2 parameters.
