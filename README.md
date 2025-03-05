# CPP02
# README: C++ Exercises - Fixed Point Arithmetic

This README provides an explanation of the theory behind the six C++ exercises related to fixed-point arithmetic. The exercises involve building a class to handle fixed-point numbers, implement various arithmetic and comparison operations, and understand how floating-point and integer types work.

---

## **Exercise 00: Mon premier canon**

### **Concepts Covered**:
- **Class Definition**: Creating a class with private and public members, including constructors and destructors.
- **Fixed-Point Representation**: Storing numbers as integers and simulating floating-point behavior with fixed-point arithmetic. This is done by scaling integer values.
- **Constructor, Destructor, and Copy Operations**: Learning how to implement constructors (default and copy), destructors, and the copy assignment operator for handling class instances.
- **Member Functions**: Defining functions like `getRawBits()` to access raw data and `setRawBits()` to modify it.

### **Explanation**:
In this exercise, you create a `Fixed` class to represent fixed-point numbers. The class will store the value as an integer, and the fixed-point representation will use 8 bits for the fractional part. You will need to implement the constructors, destructors, and a few member functions to access and modify this value. The focus is on understanding fixed-point representation and how it differs from regular floating-point numbers.

---

## **Exercise 01: Premiers pas vers une classe utile**

### **Concepts Covered**:
- **Converting Between Types**: The exercise teaches how to convert integers and floats to fixed-point numbers. It also covers converting back to float and integer types from fixed-point representation.
- **Overloading Operators**: You will overload the stream insertion operator (`<<`) to allow easy printing of `Fixed` objects.
- **Constructors**: Creating additional constructors that accept integers and floating-point numbers as input, converting them into the internal fixed-point representation.

### **Explanation**:
The goal of this exercise is to enhance the `Fixed` class to support conversions between integers, floating-point numbers, and fixed-point values. The new constructors will convert integers and floats to fixed-point format, and two member functions (`toFloat()` and `toInt()`) will perform the reverse conversions. Additionally, the class will now support printing the fixed-point values via the overloaded `<<` operator.

---

## **Exercise 02: Maintenant, on peut parler**

### **Concepts Covered**:
- **Operator Overloading**: You will overload several comparison and arithmetic operators (`>, <, >=, <=, ==, !=, +, -, *, /`).
- **Increment and Decrement Operators**: You will overload the pre- and post-increment (`++`) and pre- and post-decrement (`--`) operators to manipulate the fixed-point values.
- **Static Member Functions**: The exercise includes static member functions (`min` and `max`) that compare two `Fixed` objects and return the smaller or larger one, respectively.
- **Functionality Testing**: Ensuring all the overloaded operators and static functions work correctly.

### **Explanation**:
This exercise builds on the previous ones by adding arithmetic and comparison operations to the `Fixed` class. You will implement the arithmetic operators (`+`, `-`, `*`, `/`) to perform calculations on fixed-point values. Additionally, comparison operators (`>`, `<`, `>=`, `<=`, `==`, `!=`) will allow comparisons between two fixed-point numbers. The increment and decrement operators are overloaded to modify the fixed-point values by one unit at a time. Lastly, the static functions `min` and `max` will return the smaller or larger of two fixed-point values.

---

## **Conclusion**

These exercises guide you through the creation of a `Fixed` class to handle fixed-point arithmetic in C++. By the end of the exercises, you'll have a deep understanding of how to represent numbers in fixed-point format, overload operators for comparison and arithmetic, and implement various useful functions like `min` and `max`. These skills are crucial for working with performance-critical applications that require precise control over floating-point operations, such as in embedded systems, graphics, and scientific computing.

