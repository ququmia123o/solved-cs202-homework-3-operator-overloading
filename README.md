Download Link: https://assignmentchef.com/product/solved-cs202-homework-3-operator-overloading
<br>
<strong>Your primary goal</strong> with program #3 is to apply the functionality of the operators, the appropriate arguments (operand data types) and returned types (residual values for the operators) to the following problem. Think about how the operators are used and try to mimic the behavior in your own classes. How is the returned type used? Who controls the memory of the residual value? The client program (lvalue) or the operator (rvalue). Make sure to pass (and return) by reference whenever possible!

<strong><u>Remember OOP:</u> </strong>

With OOP the key idea is to break down the problem outlined (below) into small pieces and assign those responsibilities to individual classes. For each assignment, your job will be to create an OO design and program that shows how Object Oriented constructs could be used to solve a real-world problem. You will want to focus on how to design classes that are well structured, efficient, that work together, and where each class has a specific <strong>“job”</strong>. This time you are adding operator overloading as the new syntax for your solution!




Before you design this program, take a look back at your first two programs. Did you tie the data structures into the midst of your OO designs? Did the designs really become all about the data structure and not so much about the problem at hand? The key to OOP in my opinion is to create the design based on the problem prior to applying the data structure. The data structures are about how we handle the data – not necessarily the key to OOP. <u>For this assignment, your application</u> <u>will be the OOP portion of the assignment. Then, implement the data structures.</u>

<h1>Program #3 – The Problem</h1>

We are entering the holiday season. Do you like to get together with friends or family members? My sister always puts on some great feasts for us. Of course many of us need to consider what foods we can or should actually eat. Are there nuts? Gluten? Are there non-alcoholic choices for beverages? Many of us have dietary restrictions needing gluten free, or needing to know about the contents of nuts as well as many others. We also might need to select dishes based on their known caloric or sugar values (it is not a pretty sight when my family has too much sugar!). So, we want to develop an application that will allow a host to communicate to others what options are available.

<strong>The Data: </strong>Your job for program #3 is to create a Food data type that allows users to enter in specifics about that item in terms of common dietary restrictions. You are to support at least three different types of food items that are similar yet different (e.g., main_course, desert, beverages, etc.); the three types may be of your selection but they should have similar but yet different characteristics. At least two of your classes must support dynamically allocated data as part of the class (e.g., the name as a char *). Please have fun with these cclasses and come up with some of your own characteristics.

<strong>Making it OO:</strong> We will use this concept to develop an OO application. You will want to develop at least five classes, as normal. Make sure to use single inheritance in your design. To break down the problem, think about what is similar or different about different kinds of food characteristics. Use inheritance to push up the common elements to the base class! Then, have the derived classes handle the differences. Remember to avoid getters as much as possible with these classes – instead implement the functions that actually work ON the data IN the classes that own the data!! This is where you will get the most benefit of OOP.

<strong>Searching and the Data structure:</strong> Our data structure will be a TREE of food items that are part of the hosts planned menu.  You have an option with this – the TREE can either be implemented as a Binary Search Tree (BST) or it  can be implemented as a 2-3-4 balanced tree. If you select a BST, then a balanced tree will be assigned to you for Program #4 (in Java).  *** If you are implementing a balanced tree, you will <u>not</u> be expected to implement an individual removal operation (we will not be removing individual characteristics in a balanced tree!). <em>You can have three different data structures for the three different types of food, or you may use dynamic binding with upcasting, using just one data structure.</em>

<strong>Operator Overloading: </strong>The key part of this assignment is to implement a complete set of operators. The operators to support must include: =, +, +=, ==, !=, the relational/equality operators, and the ability to input/output data. I imagine the [] would be useful as well for searching for a match. As you decide how to apply the operators, make sure to stay within the rules of how the operators are expected to behave.




All of the aforementioned operators NEED to be implemented. But, they do not need to be implemented in the same class. <strong><u>OPERATORS DO NOT COUNT if</u> <u>they are only implemented for a ‘string-like’ class.</u></strong> Although you MAY write your own STRING data type, it can’t be the only place you use operator overloading (since the code is in topic #6!).




Of course, the = operator needs to be implemented in all classes that manage dynamic memory – and don’t forget your copy constructors!!!!




<strong>Questions to ask…about operator overloading </strong>

When using operator overloading, remember to ask yourself the following questions:

<ol>

 <li>What should be the residual value (and what data type is this)? – <em>Never have a void returning operator! </em></li>

 <li>Should the result be a modifiable lvalue or an rvalue?

  <ul>

   <li>Lvalues are returned by reference, most rvalues are returned by value. c) What are the data types of the operator’s operands?</li>

   <li>If the operand isn’t changed, then make it a const</li>

   <li>Remember to pass as a constant reference whenever possible. d) Is the first operand always an object of class?            – If so, then it could be a member function.</li>

  </ul></li>

</ol>

<ol>

 <li>e) Can the operator be used with constant operands?</li>

</ol>

– If the first operand can be a constant, and IF it is a member function, then it should be a constant member function.


