# Homework First Week

## 1 – Why we need to use OOP ? Some major OOP languages ?
</br>
	➤ Project will be more organized , you know exactly where to look when something goes wrong. This causes higher productivity and low maintenance cost.</br>
	➤ With abstraction, project will be more secure and datas will be only editable in the related class.</br>
	➤ You don't have to rewrite codes. You can reuse your code as many times as needed with Inheritance.</br>
	➤ You can extend your code without rewriting it. Through polymorphism you can add on the existing code with "method overriding".</br>
	➤ It's easier to understand, reuse and maintain.</br>
	</br>
	➤ Most popular OOP languages are Java, C++, C#, Python and Javascript.</br>
	</br>

## 2 – Interface vs Abstract class ? 
</br>

**Interface**
</br>
	➤ There is no code inside the methods and only method definitions.</br>
	➤ Access modifiers are not used. Everything is considered public.</br>
	➤ Multiple inheritance can be used</br>
	</br>
**Abstract class**
</br>
	➤ Used for gather the objects that have in common.</br>
	➤ Used in Is-A relationships and extended class takes all the features.</br>
	➤ Methods and variables can be defined.</br>
	</br>
	
## 3 – Why we need equals and hashcode ? When to override ?
</br>
	➤ With the Equals method, we get a boolean return that two objects are equal to each other.</br>
	➤ If two objects are equal according to equals() method, then their hash code must be same.</br>
	➤ But if two objects unequal according to equals() method, their hash code are not required to be different.</br>
	➤ So we should use the equals method first and then the hashCode() method. But there is something we should know.</br>
	➤ If we are not planning to use the class as Hash table key, then our program will not throw any exceptions.</br>
   	➤ If we are going to use a class as Hash table key, then it's must to override both equals() and hashCode() methods.</br>
	</br>

## 4 – Diamond problem in Java ? How to fix it? 
</br>
	➤ Java does not allow multiple inheritance where one class can inherit properties from more than one class. </br>
	➤ This is known as Diamond problem.</br>
	➤ Because of the interfaces can do multiple inheritance, we can achieve Diamond problem by using interfaces and default methods. </br>
</br>

## 5 – Why we need Garbagge Collector ? How does it run ? 
</br>
	➤ Understanding Garbage Collector means writing better and more effective Java applications.</br>
	➤ Automatically handles the deletion of unused objects or objects that are out of reach to free up vital memory resources. </br>
	➤ The space occupied by unused/non-referenced objects are detach from memory and cleared from memory.</br>
	➤ The mechanism that performs this operation is called the Garbage Collector.</br>
	</br>
	
## 6 – Java ‘static’ keyword usage ?
</br>
	➤ The static keyword in Java is used for memory management mainly.</br>
	➤ We can use static keyword with variables, methods, blocks and nested classes.</br>
	➤ It makes your program memory efficient. </br>
	➤ Static variable will get the memory only once, it will retain its value.</br>
	➤ In static method, we don't have to create instance of a class. It's belongs to the class rather than the object of a class.</br>
	➤ The static method can't use non-static contexts.</br>
	➤ this and super keywors can't be used in static methods.</br>
	➤ Static block is executed before main method, used to initialize the static data member.</br>
</br>

## 7 – Immutability means ? Where, How and Why to use it ? 
</br>
	➤ Immutability means that we can not change its content. </br>
	➤ In Java, immutable class must be initialize as final so child classes can't be created.</br>
	➤ Datas in this class must be declared as private final because direct access is not allowed and we can't change the value after the creation.</br>
	➤ Must have getter methods and they can't have setter methods or any method that can change the value of the datas.</br>
	➤ In immutable class, data won't change. Once verified, it will be valid. Better cacheability.</br>
</br>

## 8 – Composition and Aggregation means and differences ? 
</br>
	➤ They are two types of association which is used to represent relationships between two(parent-child) classes. </br>
	➤ In composition, there is strong relationship between these two classes. Parent class owns the child class. In UML diagram it is denoted by filled diamond.</br>
	➤ In aggregation, there is weak relationship between these two classes. </br> 
	➤ There is Has-A relationship, which doesn't imply ownership. In UML diagram it is denoted by empty diamond.</br>
</br>

## 9 – Cohesion and Coupling means and differences ? 
</br>
	➤ Cohesion refers to what the class (or module) can do.</br>
	➤ Low cohesion focuses on what actions it involves, not what it does and what it contains.</br>
	➤ High cohesion focuses on what it should be doing,with only methods relating to the intention of the class.</br>
	➤ Coupling, refers to how related or dependent two classes/modules are toward each other.</br>
	➤ For low coupled changing something will not affect the other. In other hand for high coupled, change will be majorly impact the other.</br>
	➤ Because of this, good software design has high cohesion and low coupling.</br>
	</br>
	
## 10 - Heap and Stack means and differences ?
</br>
	➤ Memory management in Java handled by itself. The JVM divides the memory into two parts stack memory and heap memory.</br>
	➤ Stack is used to store the order of method execution and local variables while the heap memory stores the objects and it uses dynamic memory allocation and deallocation.</br>
	➤ Stack stores the variables, references to objects, and partial results.</br>
	➤ The stack memory is a physical space (in RAM) allocated to each thread at run time.</br>
	➤ Stack follows LIFO (Last-In-First-Out) order.</br>
	➤ Heap memory stores objects and JRE classes.</br>
	➤ Heap does not follow any order like the stack.</br>
	➤ Managing the memory automatically, by garbage collector that deletes the objects which are no longer being used.</br>
	➤ The elements are globally accessible.</br>
</br>

## 11 – Exception means ? Type of Exceptions ?
</br>
	➤ An event that occurs during the execution of a program that disrupts the normal flow of instructions is called an exception.</br>
	➤ Exceptions that are already available in Java libraries are referred to as built➤in exception.</br>
	➤ There is also user-defined exception which in that case we want the program throw that exception.</br>
	➤ SQLException → Occurs while executing queries on a database related to the SQL syntax.</br>
	➤ IOException → Occurs while using file Input-Output stream operations.</br>
	➤ ArrayIndexOutofBound → Occurs when you try to access an array with an invalid index value.</br>
	➤ IllegalArgumentException → Occurs whenever an inappropriate or incorrect argument is passed to a method.</br>
	➤ NullPointerException → Occurs when you try to access an object with the help of a reference variable whose current value is null or empty. </br>
	➤ This is the java exception hierarchy.</br>
	
![hierarchy-of-exception-handling](https://user-images.githubusercontent.com/88919177/149395577-633b0586-9317-4648-9284-584c9810c25f.png)

	
## 12 – How to summarize ‘clean code’ as short as possible ? 
</br>
	➤ Clean code is code that is easy to understand and easy to change.</br>
	➤ Code is easy to extend and refactor, and it’s easy to fix bugs in the codebase. </br>
</br>

## 13 - What is the method of hiding in Java ? 
</br>
	➤ If a subclass defines a static method with the same signature as a static method in the super class in such a case, the method in the subclass hides the one in the superclass.</br>
	➤ The mechanism is known as method hiding. It happens because static methods are resolved at compile time and can't be overridden.</br>
	➤ Difference between the method overriding is methods are static, not instance.</br>
	</br>
	
## 14 - What is the difference between abstraction and polymorphism in Java ? 
</br>
	➤ Abstraction hides the unnecessary detail but shows the essential information.</br>
	➤ Abstraction focuses on the external lookout while encapsulation focuses on internal working.</br>
	➤ Encapsulation hides the code and data into a single entity or unit.</br>
	➤ The objects are encapsulated that helps to perform abstraction.</br>
