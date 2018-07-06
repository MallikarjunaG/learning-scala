## Scala Overview

* Scala is general purpose programming language.
* Scala stands for Scalable Language
* Scala was designed by Martin Odersky. 
* Scala was officially released in early 2004.
* Scala is an object-oriented and functional programming language.
* Scala is modern multi paradigm and hybrid programming language.
* Scala integrates the features of object-oriented and functional languages.
* Scala is designed to express common programming patterns in a concise, elegant, and type-safe way.
* Scala design was inspired by Java and Lisp.
* Scala is a strong static type language.
* In scala, everything is an object whether it is a function or a value. 
* Scala does not have support primitive data types.
* Scala source file having an extension of either .scala or .sc.
* Scala is interactive programming language.
* Scala is hybrid Programming language
* Scala is compiled to run on the Java Virtual Machine (JVM)
* Scala is crisp, productive, interactive, Scalability and Reliability
* Scala is interoperable with Java Library.
* Scala allows development in two ways:
  * Interactive Mode
  * Standalone
* We can use Scala for developing following type of applications.
  * Web applications
  * Enterprise applications
  * Mobile applications
  * Desktop applications
  * Data Analysis applications
  * Utilities and Libraries
  * Streaming Applications
  * Parallel and batch processing applications
  * etc...
* Scala is crisp, productive and easy to learn.
* Scala is not extension of Java, but it is interoperable with Java.
* Scala is pure object oriented and functional oriented programming language.
* Scala is a pure object oriented language in the sense that every value is an object
* Scala is pure functional language in the sense that every function is a value.

#### Scala Hello World Progrom:
```
  Interactive Mode using scala, scala notebook, zeppelin etc...
  
     println("Hello World")
     
  Standalone Mode:
  
  object HelloWorld {
    def main(args:Array[String]) {
       println("Hello World")
    }
  }
```
**************

## Scala Features:
* Scala is Object Oriented
  * Scala is pure object oriented
  * Every value is scala is an Object
  * Scala Function also is an Object
  * Subclassing
  * Mixin-based composition -- Multiple inheritance
* Scala is Functional
  * In Scala, every function is an object
  * Ananymous Functions
  * Higher- Order functions
  * Nested
  * Currying
* Type inference: Scala offers Type Inference i.e., no need to provide the data type explicitly
* Singleton objects: Scala offers Singleton i.e., no static members.
* Immutability: Scala offers Immutability i.e., can not modify variable values.
* Lazy computation: Scala offers Lazy computation i.e., it evaluates expressions only when they are required.
* Case classes and Pattern matching: Scala case classes are regular classes but there are immutable. Scala case classes are used in combination with Scala pattern matching.
* Concurrency control: Scala provides actor model for better handling of Concurrency.
* String interpolation: Scala String interpolation allows embedding variables as part of Scala string.
* Higher order function: Scala offers high order functions i.e., function takes another function as argument or function returns another function as return value.
* Traits: Scala provides trait which contains fields and methods of type abstract and non abstract.
* Rich collection set: Scala provides a rich set of mutable and immutable collections to manipulate the data.
* Closures: Scala offers ananymous functions
* etc...
******************************************

## Scala Installation:
* Scala requires Java JDK
* Download Java JDK and Install it
* Add JAVA_HOME
* Download Scala based on OS
* Add SCALA_HOME
* Add Scala executables and Java Executables into the System PATH variable in the .bashrc file.
### Checking Scala and Java Installations:
 ```
  > java -version
  > javac -version
  > scala -version
  > scalac -version
  ```
 ## Scala IDEs
 * Scala Eclipse (Standalone)
 * Scala Shell (Interactive)
 * Scala Notebook (Interactive)
 * Zepplein Notebook (Interactive)
 * Sublime Text Editor (Standalone)
 * Vim/Vi Editor (Standalone)
 * InteliJ (Standalone)
 * Many more editors
********************

## Scala Variables and Data Types
* Scala allows two types of variables i.e., val and var
* val is constant i.e., immutable
* var is modifiable i.e., mutable.

```
val name = "Naga"
name = "Ravi" // This throws error

var age = 30
age = 35 // This works
```
* The following are standard data types in Scala which are similar to Java. The only difference is which are Objects rather than primitives.
  * Byte
  * Short
  * Int
  * Long
  * Float
  * Double
  * String
  * Char
  * Boolean
  * Null
  * Nothing
  * Any
  * AnyRef
  * AnyVal
  * etc...

*******************
## Scala Control structures:
* Scala offers the following control structures which are used control flow of Scala program.
  * Conditional Statements
    * if, if-else, nested if-else, if-else ladder
  * Scala Pattern Matching
  * Scala loops

#### Conditional Statements:
##### if-statement
```
   Syntax:
   if(<condition>){
    statements...
   }
```
##### if-else statement
```
if(<condition>){
 statements...
}else{
 statements....
}
```
##### if-else ladder
```
if(<condition>){
 statements...
}else if(<condition>){
 statements....
}else if(<condition>){
 statements..
}else{
 statements....
```
*Note: Use Ternary operator instead of if-else statements i.e., ```<condition> ? <true case> : <false case>```*
#### Scala Pattern Matching:
* Scala pattern matching is alternative to switch statement.
```
variable match {
case 1 => statements
case 2 => statements
case 3 => statements
case _ => statements
}
```
#### Loops
* while loop
* do while loop
* for loop
```
while loop:

while(<condition>){
 statements
}

do-while loop:

do{
 statements
}while(<Condition>)

for loop:

for(i <- range){
 statements
}

for(i <- ScalaCollection){
 statements...
}
```

*********************
## Scala Comments
* Scala supports thre types of comments
  * Single line ```//```
  * Multi line ```/*....*/```
  * Documentation ```/** **** */```
  
***************
## Scala Functions
* Scala supports functional programming
* Scala has lot of builtin functions and also supports for user defined functions.
* Scala Functions are first class values.
* Store Scala Function as value
* Every value in Scala is an Object i.e., Scala function also an Object.
* Scala allows passing a function as method/function argument and return function as another function return value.
* Scala functions are defined with keyword *def* like in Python and Ruby.

#### Scala Function Definition:
```
def functionName([funcParams : typeofparameters]) : [returntypeoffunction] = {  
statements...
[(return_value)]
}
```
#### Higher Order Functions:
* Scala higher order function is a function that either takes a function as argument or returns a function
```
def functionName(<another function>) : <another function> = {
 statements.....
}

```

****************************
## Scala Classes and Objects
* Scala is pure Object oriented programming language
* Object is a real world entity. It contains state and behaviour
* Class is a blueprint/template of an Object.
* Scala class contains the following things:
  * Data member
  * Member method
  * Constructor
  * Block
  * Nested class
  * Super class information
* In Scala, the default scope is public

```
Class:

class Employee{
var name:String = null
var age:Int = 0
}

Object

object EmpExample{
 def main(args:Array[String]) {
  val emp = new Employee()
  println(emp.name)
  println(emp.age)
 }
}


class Employee(name:String, age:Int){
 def getName():String = {
  (name)
 }
 def getAge():Int = {
 (age)
 }
}

Object

object EmpExample{
 def main(args:Array[String]) {
  val emp = new Employee("Naga", 30)
  println(emp.name)
  println(emp.age)
  println(emp.getName)
  println(emp.getAge)
  println(new Employee("Rajesh", 40).getName()) // Ananymous Object
 }
}
```
### Singleton and Companion object
* Singleton object is an object which is declared by using object keyword instead by class.
* In Scala, there is no static concept. So scala creates a singleton object to provide entry point for your program execution.
* Methods declared inside Singleton Object are accessible globally.
* Singleton object can extend classes and traits.
```
object SingletonObjectName {
variables + methods
}
```
* In scala, when you have a class with same name as singleton object, it is called companion class and the singleton object is called companion object.
* Both the companion class and its companion object both must be defined in the same source file.
```
Hello.scala

object Hello {
 def main(args:Array[String]){
   val hello = new Hello()
   hello.message()
 }
}

class Hello {
 def message(){
  println("Hello")
 }
}
```
### Scala Case class and Case Object
* Scala case classes are just regular classes which are immutable by default and decomposable through pattern matching.
* Scala case class uses equal method to compare instance structurally. 
* Case class does not use new keyword to instantiate object.
* All the parameters listed in the case class are public and immutable by default.

```
case class Person(name:String, age:Int)

object PersonExample {
 def main(args:Array[String]){
  val person = Person("Naga", 30)
  println(person.name)
  println(person.age)
 }
}
```
### Scala case class and pattern matching:
```
abstract class Notify
case class Email(from:String, to:String, message:String) extends Notify
case class SMS(to:String, message:String) extends Notify
case class Alert(message:String) extends Notify

def sendNotification(notification:Notify) : Unit = notification match{
    case Email(from, to, title) => println("You got a mail")
    case SMS(to, msg) => println("You got an SMS")
    case Alert(msg) => println("You got an Alert")
    case _ => println("No Event")
}

val email = Email("abc@gmail.com", "xyz@gmail.com", "HI How are you?")
sendNotification(email)
```
### Scala Constructors:
* Scala provides primary and auxiliary constructors.
#### Scala default primary constructor:
* This is the default constructor, no need to specify the default primary constructor.
```
class Employee{
 println("Employee...")
}

object Emp{
  def main(args:Array[String]){
   val emp = new Employee()
  }
}
```
#### Scala primary constructor:
* Scala allows to define primary constructor with zero or more parameters with definition of the class.
```
class Employee(name:String, age:Int){
 def getName(): String = {
  (name)
 }
 def getAge(): Int = {
  (age)
 }
}
```
#### Scala Secondary or auxiliary Constructor:
* We can create any number of auxiliary constructors in a class.
* We must call primary constructor from inside the auxiliary constructor.
* this keyword is used to call constructor from other constructor.
```
class Employee(name:String, age:Int){
 var place = ""
 def this(name:String, age:Int, place:String){
     this(name, age)
     this.place = place
 }
 def getName(): String = {
  (name)
 }
 def getAge(): Int = {
  (age)
 }
 def getPlace():String = {
     (place)
 }
}

object Emp {
def main(args:Array[String]){
val emp = new Employee("Naga", 30)
val employee = new Employee("Ravi", 33, "Mysore")
println(emp.getName())
println(employee.getPlace())
}
}
```
### Scala Method Overloading
* Scala offers method overloading
```
class Maths{
 def add(a:Int, b:Int) : Int = {
  (a + b)
 }
 def add(a:Int, b:Int, c:Int) :Int = {
  (a + b + c)
 }
}
```
## scala this keyword:
* this is a keyword and used to refer current object.
```
class Employee{
    var name = ""
    var age = 0
    var place = ""
    def this(name:String, age:Int, place:String){
        this()
        this.name = name
        this.age = age
        this.place = place
    }
}
```
## Scala Inheritance
* Inheritance is an object oriented concept which is used to reusability of code. 
* We can achieve inheritance by using extends keyword.

```
class Programmer extends Employee{
 //Write code....
}
class Employee{
  var name = ""
  var age = 0
}

class Programmer extends Employee {
 var bonus = 0.0
}
```
## Scala Method Overriding
* If subclass has the same name method as defined in the parent class, it is known as method overriding
```
class Employee{
  def message(){
  }
}

class Programmer extends Employee {
 override def message(){
  println("You are a Programmer")
 }
}
```
## Scala Field Overriding:
*  mutable variable cannot be override, only immutable variables are overridden
```
class Employee{
    val age = 30
    def message(){
        
    }
}

class Programmer extends Employee{
    override val age = 40
    override def message(){
        println("You are Programmer")
    }
}

val programmer = new Programmer()
println(programmer.age)
programmer.message()
```
## Scala final keyword:
* In Scala, final is a keyword, which is used to prevent inheritance of super class members into derived class.
* We can declare final variables, methods and classes also.

## Scala Abstract Class:
* Scala class which is declared with abstract keyword is known as abstract class.
* An abstract class can have abstract methods and non-abstract methods as well.
* Abstract class is used to achieve abstraction.
* Abstraction is a process in which we hide complex implementation details and show only functionality to the user.
* In scala, we can achieve abstraction by using abstract class and trait.

```
abstract class Employee{
    def getName() : String
    def getAge() :Int
}

class Manager(name:String, age:Int) extends Employee {
    def getName() : String = {
        (name)
    }
    def getAge() : Int = {
       (age)
    }
}

val manager = new Manager("Arjun", 35)
println(manager.getName)
println(manager.getAge)
```
## Scala Trait
* Scala trait is like an interface with a partial implementation. 
* Scala trait is a collection of abstract and non-abstract methods.
```
trait Shape{
    def area(x:Double) : Double
}

class Square extends Shape {
    def area(x:Double) : Double = {
        (x * x)
    }
}

val square = new Square()
val aread = square.area(10.0)

MixIns:

trait Shape{
    def area(x:Double, y:Double) : Double
}

trait Printable{
    def printShape(shape:String)
}

class Rectangle extends Shape with Printable{
    def printShape(shape:String) {
        println("The shape type is: " + shape)
    }
    def area(x:Double, y:Double) : Double = {
        (x * y)
    }
}

val rectangle = new Rectangle()
rectangle.printShape("Rectangle")
val area = rectangle.area(10.0, 20.0)
println("Area of rectangle is: " + area)

``` 
***********************
## Scala Arrays:
* Scala array is a collection of mutable values.
* Index starts from 0 and last index is n-1
* Scala arrays are generic i.e., Array[T]
* Scala arrays are compatiable with Scala Sequences
* Scala supports two types of arrays:
  * One dimensional
  * Multi dimensional
### One Dimensional Array:
```
val varName:Array[arrayType] = new Array[arrayType](arraySize)
val varName = new Array[arrayType](arraySize)
val varName:Array[arrayType] = new Array(arraySize)
val varName = Array(e1,e2,e3,....eN)

val names = Array("Naga", "Ravi", "Kiran")
val numbers = new Array[Int](10)

for(i <- 0 until 10){
    numbers(i) = i
}

for(num <- numbers){
    println(num)
}

```
### Multi Dimensional Array:
```
var arrayName = Array.ofDim[ArrayType](r,c)   //r = rows, c = columns
var arrayName = Array(Array(e1,e2...eN), Array(e1, e2, ....eN))

val matrix = Array.ofDim[Int](2,2)
matrix(0)(0) = 1
matrix(0)(1) = 2
matrix(1)(0) = 3
matrix(1)(1) = 4

println(matrix(1)(1))

val persons = Array(Array("Naga", "Ravi"), Array(30, 33))
println(persons(0)(0))
println(persons(0)(1))
println(persons(1)(0))
```
**********************
## Scala Strings:
* In Scala, string is a combination of characters or we can say it is a sequence of characters.
* Strings are immutable
* We can manipulate string and can apply method to get desire results.
* We can't change original string object.
```
val firstName = "Arjun"
val surName = "A"
val name = firstName + " " + surName
val fullName = firstName.concat(surName)
println(name)
println(fullName)

String Comparision:

val name = "Naga"
val name1 = "Naga"
if(name == name1){
    println("Equal")
}else{
    println("Not Equal")
}

String Interpolation:

val name = "Naga"
println("Name: " + name)
println(s"Name: $name")

var message = raw"naga\t30\tbangalore\n"
println(message)
```
***********************
## Scala Exceptiona Handling:
* Exception handling is a mechanism which is used to handle abnormal conditions.
* We can avoid termination of your program unexpectedly.
* Scala doesn't have checked exceptions.
* All Exceptions are unchecked exceptions.
```
class Maths{
    def divide(nums:Array[Int]){
          for(num <- nums){
            try{
            val division = 100 / num
            println(division)
            }catch{
            case ae:ArithmeticException => println(ae.getMessage())
            case e:Exception => println(e.getMessage())
            }
            finally{  
            println("Finaly block always executes")  
        }  
        }   
    }
}

val math = new Maths()
val numbers = Array(1,2,3,4,5,0,6,7,8,9)
math.divide(numbers)

Scala throw keyword: The throw keyword mainly used to throw custom exception.

class Vote{
    def validate(age:Int){
        if(age <= 18){
            throw new ArithmeticException("You are not eligible for voting!")
        }else{
            println("You are eligible for voting!")
        }
    }
}

val vote = new Vote()
vote.validate(12)

Scala throws Keyword: We can declare exception with method definition using throws keyword.

class StrToNum{
    @throws(classOf[NumberFormatException])
    def strToNum(number:String){
        val num:Int = number.toInt
        println(num)
    }
}
val sn = new StrToNum()
sn.strToNum("ABC")

```
*******************
## Scala Collections:
* Scala provides a rich set of collections library.
* Scala collection library contains Classes and traits.
* Scala collection library contains both mutable and immutable collections.
  * scala.collection.mutable
  * scala.collection.immutable
* Traversab le is a base trait in scala immutable collection library.
* Traversable is used to traverse collection elements.
* Scala Iterable is a trait for iterable collections.
#### Set:
* Used to store unique elements in the set.
* It does not maintain any order for storing elements.
```
val names:Set[Type] = Set(e1,e2,....eN)
val names = Set(e1,e2,....eN)

val names = Set("naga", "ravi", "hari")

//merge two sets
val names = Set("naga", "ravi", "hari", "ravi")
val names1 = Set("kiran", "kishore", "ashok", "amit")
val namesList = names ++ names1
namesList

//Adding and removing elements
var names = Set("naga", "ravi", "hari", "ravi")
println(names)
names += "siva"
println(names)
names -= "ravi"
println(names)

//Iterating over sets
for(name <- names){
    println(name)
}

names.foreach(item => println(item))

//set operations
val A = Set("a", "b", "c", "d")
val B = Set("c", "d", "e", "f")

val intersection = A.intersect(B)
val union = A.union(B)
println(intersection)
println(union)
```
#### SortedSet:
* set values are sorted in Order.
```
val varname:SortedSet[Type] = SortedSet(e1, e3, e2, ..., eN)
val varname = SortedSet(e1, e3, e2, ..., eN)

import scala.collection.immutable.SortedSet

val numbers = SortedSet(2,4,3,1,6,5,7,9,8)
println(numbers)
```





## Additions

## Scala Classes:
* Scala class is blue print/template for scala Object
* Scala Object is instance of class.
* Scala Objects are created from Scala class using "new" operator
* Scala class contins state (data member) and behavior (Member function)
* In Scala Class, we have fields and methods

Class Example
```
class Employee(name:String, age:Int, role:String) {
  val this.name = name
  val this.age = age
  val this.role = role
  def getName() : String = {
    return name
  }
  def getAge() : Int = {
    (age)
  }
  def getRole(): String = {
    (role)
  }
  
}

Object Example:

object Emp {
  def main(args:Array[String]) : Unit = {
    val emp = new Employee("Naga", 30, "Architect")
    println(emp.getName)
    println(emp.getAge)
    println(emp.getRole)
  }
}

Extending Classes:

class Manager(name:String, age:Int, role:String, team:String) extends Employee(name:String, age:Int, role:String){
    val this.team = team
    def getTeam() : String = {
        return team
    }
}

object Emp {
  def main(args:Array[String]) : Unit = {
    val emp = new Manager("Naga", 30, "Architect", "Hadoop")
    println(emp.getName)
    println(emp.getAge)
    println(emp.getRole)
    println(emp.getTeam)
  }
}
```
## Singleton Objects:
* Scala is pure Object Oriented and there are no static members.
* Scala has Singleton objects instead of static memners.
* Singleton is class that can have only one instance of Object.
* We create singleton using the keyword object instead of class keyword.
* There is no instantiation and there is no parameters passing to constructor.
```
Example:
object Hello {
  def main(args:Array[String]){
    println("Hai")
  }
}
```
## Access Modifiers:

* There are three types:
  * public i.e., default no need to specify
  * private
  * protected
```
class Employee {
.....
}

The class is public here....

class Employee {
   private var name:String = null
   private var age:Int = 0
   private var place:String = null
   
   def setName(name:String) = {
    this.name = name
   }
   def getName(): String = {
       (this.name)
   }
}

object Emp {
  def main(args:Array[String]) {
    val emp = new Employee()
    emp.setName("Naga")
    println(emp.getName)
  }
}
```

## Scala Control Structures:
* Branching
  if-else
```
  if (<condition>){
  }
  
  val a = 10
  if(a < 20){
    println("Hai")
  }
  
  val a = 30
  if (a < 20 ){
    println("hai")
  }else{
    println("Bye")
  }
```
* Looping
  * for loop:
   ```
    for( var varName <- []){
      statements.....
    }
    
    for(i <- 1 to 10){
        println(i)
    }
    
    for(i <- 1 until 10){
      println(i)
    }

    val names = List("ravi", "hari", "siva", "rajesh")
    for(name <- names){
      println(name)
    }
    
    val numbers = List(1,2,3,4,5,6,7,8,9)
    val even = for(num <- numbers if num % 2 == 0) yield num
    
    for(num <- even){
      println(num)
    }
   ```
   * while loop:
   ```
    while(<condition>){
      statements...
    }
    
    var a = 0
    while( a < 20){
      println(a)
      a = a + 1
    }
   ```
   * do-while loop:
   ```
    do{
      statements
    } while(<condition>)
    
    val a = 20
    do {
      println(a)
    }while(a > 20)
   ```

## Scala Data Types:
* In Scala, every data type is an Object
* Scala has the following data types:
  * Byte (1 Byte)
  * Short (2 Bytes)
  * Int (4 Bytes)
  * Long (8 Bytes)
  * Float (4 Bytes)
  * Double (8 Bytes)
  * Char
  * String
  * Boolean
  * Unit
  * Null
  * Any
  * AnyRef
* Scala Literals:
  * Integer:
    10, 200L
  * Floating:
    1.0f, 0.0
  * Boolean:
    true/false
  * Char:
    'a', 'b'
  * String:
    * Single line:
      "Ravi"
    * Multi line:
      """This scala
      Tutorial.
      """

## Scala Functions:
* Scala function is a group of statements that performs a task. 
* We can divide the code into separate functions such that each function performs a specific task.
* There is minor difference between scala methods and functions.
	* A method is the one which is part of a class and has name and signature where as scala function is an object that
could be assigned to a variable.
	* In simple words to say, function defined as member of some object is called a method.
* Scala also has support for nested functions.
* Scala Function definition:
```
def functionName ([list of parameters]) : [return type] = {
   function body
   return [expr]
}
    [OR]
def functionName ([list of parameters]) : [return type] = {
   function body
   ([expr])
}

Here return type could be any valid scala data type. list of parameters would be list of variables separated by comma.
return type and list of parameters are optional.

Example of a function with return type:

object SumExample{
def main(args:Array[String]) : Unit = {
  println(sum(30, 40))
}
def sum(a:Int, b:Int) : Int = {
    return (a + b)
   }
 }
```
* Function which returns nothing can return Unit that is equivalent to void in Java.
* Funtions that donot return anything are called Procedures.
```
Example of a function that returns nothing:
object Hello{
   def main(args:Array[String]) : Unit = {
      printMe()
   }
   def printMe() : Unit = {
      println("Hello, Scala!")
   }
}
```

* Functions call-by-name:
	* Typically, the parameters of the function would be by-value parameters which means the value of the parameter is 
determined before it is passed to the function.
	* Suppose if we would need a function that accepts an expression as a parameter which will not be evaluated until it 
is called within our function. To support this feature, scala offers call-by-name parameters.
```
Example:
object CallByName
{
  def main(args:Array[String])
   {
    delayed(calc());

   }
     def calc() :Int={
	
         println("In calc function...");
         return 9
	 }
   def delayed(t: => Int)
   {
    println("In delayed method..");
    print ("Parameter value is.."+t)
   }
}

Output:
In delayed method..
In calc function...
Parameter value is..9

In the above example calc() is the parameter to delayed() function. 
Once the delayed is invoked, the message : "In delayed method" is printed indicating that delayed() has been entered.
Now, while executing second print statement in delayed() (the execution takes place from right to left), the 
parameter 't'indicates the value being returned from calc. Hence calc() is entered and displays the message 
"In calc function...". The returned value 9 is printed as 
"Parameter value is...9

Funtion with variable number of arguments:
The last parameter to a funtion may be repeated. We can variable length arguments list to the function.
Example:
def printArgs(a:Int, args:String*)
{
  a=10;
  println("Value of a is...."+a);
  for(arg<-args)
  {
    println(arg);
  }
}

printArgs(10,"hello","hi')

Result:
Value of a is....10
hello
hi

a is intialized to 10 and all the remaining arguments are considered as args.
Here args declared as String* is actually an Array[String]. Also, note that the variable args is specified in the last.
Ordinary arguments specified after varargs would lead to an error.
Example:
def VarArgs_NormPars(args:String*,a:Int)
     | {
     |   println("Integer is.."+a);
     |   for(arg<-args)
     |   {
     |     println("Arg value is..."+arg);
     |   }
     | }

Result:
<console>:7: error: *-parameter must come last
       def VarArgs_NormPars(args:String*,a:Int)


Scala lets us specify default values for the function parameters. The arguments for such parameters can be omitted 
in which case, default value would be taken.
Example:
object Test {
   def main(args: Array[String]) {
        println( "Returned Value : " + addInt() );
   }
   def addInt( a:Int=5, b:Int=7 ) : Int = {
      var sum:Int = 0
      sum = a + b

      return sum
   }
}
```

## Closures:
* Scala closure is a function, whose return value depends on the value of one or more variables declared outside this function.
```
	val a = 20
	val sum = (b:Int) => b + a
	sum(30)
	res17: Int = 50
```





## Scala Basics:
* Scala Syntax is very similar to Ruby
* Scala doesn't require semicolon(;) at end of the statement i.e., optional
* Scala has the following language components:
  * Class
  * Object
  * Method
  * Function
  * Closure
  * Traits
* We do Scala programming in two days:
  * Interactive Mode
  * Script Mode
* Scala scripts or programs have an extension of ".scala"
* Scala is case sensitive
* Scala follows Java convensions
* Scala doesn't have static members
* Scala identifiers are used for object, class, method, variable names etc...
  * Legal Identifiers
    name, place, _city, _a_salary
  * Illegal Identifiers
    $name, 1place, -salary
* Scala has many language specific reserved keywords
  * case, class, object, return, if, else, etc...
* Scala supports two types comments like Java
  * Single line comments i.e., //
  * Multiline comments i.e., /*....*/
* Scala is a line-oriented language where statements may be terminated by semicolons (;) or newlines.
* In Scala, semicolon at the end of a statement is usually optional.
* Scala organizes its classes and objects in terms of packages like Java.

### Scala Hello World Program:

##### Interactive Mode:
    ```
    println("Hello World")
    ```
##### Script Mode:
    ```
    object Hello {
      def main(args:Array[String]) {
        println("Hello World")
      }
    }
```

## Scala variables:
* Scala supports two types of variables of any data type.
  * var -- Mutable variables i.e., reassignment
  * val -- Immutable variables i.e., constant
* Scala variable declarations:
```
var variableName: [Data Type] = <value>
val variableName: [Data Type] = <value>

Example:
  var name: String = "ravi"
  var name = "hari" --> Type Inference
  
  val number: Int = 10
  val number = 10 --> Type Inference
  
  val (name: String, age:Int) = Pair("Ravi", 30)
   val (name, age) = Pair("Ravi", 30) --> Type Inference
```

### Variable Scope:
 * Fields:
   * Fields are varibales belong to Object
   * Access inside and outside
   * vals and vars i.e., mutable and immutable
 * Method Parameters:
   * Method arguments
   * Only vals i.e., always Immutable
   * Inside method
 * Local variables:
   * Declared inside the method
   * vals and vars i.e., mutable and immutable
   * Inside the method
