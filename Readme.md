# Chapter 3: Processing Data

## Objectives

This chapter introduces the basic concepts of processing data in C# Windows Forms applications. By the end of this chapter, I will understand how to:

* Read user input using TextBox controls.
* Declare and use variables.
* Work with different data types.
* Perform basic calculations.
* Convert and display numeric values.


## Topics

* 3.1 Reading Input with TextBox Controls
* 3.2 A First Look at Variables
* 3.3 Numeric Data Types and Variables
* 3.4 Performing Calculations
* 3.5 Inputting and Outputting Numeric Values
* 3.6 Formatting Numbers with the ToString() Method
* 3.7 Simple Exception Handling
* 3.8 Using Named Constants
* 3.9 Declaring Variables as Fields
* 3.10 Using the Math Class
* 3.11 More GUI Details
* 3.12 Using the Debugger to Locate Logic Errors

## 3.1 Reading Input with TextBox Controls

A **TextBox** is a Windows Forms control that allows the user to enter information using the keyboard. It can be added from the Common Controls section of the Toolbox.

The user's input is stored in the TextBox's  Text property.


string name = nameTextBox.Text;


The Text property stores input as a **string**. A TextBox can also be cleared using:

`
nameTextBox.Clear();


or:


nameTextBox.Text = string.Empty;


## 3.2 A First Look at Variables

A **variable** is a storage location in memory used to hold data. A variable name represents that memory location.

Before using a variable, it must be declared with a data type.

### Syntax


DataType VariableName;


Example:


string name;
int age;


### Data Types

The data type specifies what kind of data a variable can hold. Common types include:

* string → stores characters/text.
* int → stores whole numbers.
* double → stores numbers that can contain decimal values.
* decimal → stores decimal values with greater precision and is commonly used for financial applications.

### String Variables

A string contains a combination of characters.


string university = "Jamhuuriya University";


Strings can also be combined using the `+` operator. This is called string concatenation.


string fullName = firstName + " " + lastName;


### Variable Naming Rules

* The first character must be a letter or `_`.
* Names cannot contain spaces.
* Reserved keywords cannot be used as variable names.
* Meaningful variable names should be used.

### Local Variables and Scope

A local variable belongs to the method where it is declared. Only statements inside that method can access it.

Scope refers to the part of the program where a variable can be accessed.

A local variable must also be assigned a value before it is used.





