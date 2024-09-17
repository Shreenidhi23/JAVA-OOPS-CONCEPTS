# JAVA-OOPS-CONCEPTS
#CLASS
#OBJECT
#ENCAPSULATION
#ABSTRACTION
#INHERITENCE
#POLYMORPHISM

>>>>>>>CLASS<<<<<<
#CLASS is a template for objects and it is a blueprint from which you can create an individual object.
#SYNTAX
 class class_name                   
{
    data members
    member functions
}
#EXAMPLE
class Student
{
  int id;     //data member
   //member function
  void display()
 {
System.out.println(id);
 }
}
>>>>>>>OBJECT<<<<<<
#OBJECT An instance of class , representing a real-world entity or concept,with its own:[ It has state and behaviour]
$$ State - attributes/properties-Data stored within the object.
$$ Behaviour(methods): Actions performed by the object.
#SYNTAX
class_name object_name=new class_name();
#Example
    Student s1 = new Student();
>>>>>>>![oops-object](https://github.com/user-attachments/assets/4cb662a0-d09b-4664-8d27-26f7f5dfb9c7)<<<<

>>>>>>>ENCAPSULATION<<<
#Encapsulation is combining/encapsulating data and function in single unit.
#It is hiding/functions within a class and controlling access using acess specifiers.
______________________________
|  >>>VARIABLES/ DATA<<< |   
|  >>>METHODS/ FUNCTION << |  >> *CLASS*--Encapsulating data and functions in a SINGLE UNIT.
________________________________
#SYNTAX
class class_name
{
(private/public/protected) data members
    member functions
}
#Example 1:
class Student
{
  private int id; //data member
  //member function
  private void display()
  {
  System.out.println(id);
  }
}
#Example 2.1:
package college;

  int id; //data member
  // member function /method
  void display()
  {
       System.out.println(id);
  }
  public static void main(String[] args) {
      Student obj=new Student();
      obj.id=90;
      obj.display();
      Student_1 obj 1=new Student_1();
      obj1.
    }
   }
2.2 - 
package college;
 private int marks;
 private void displayMarks()
 {
    System,out.println(marks);
 }  
}

>>>>INHERITENCE<<<<
#INHERITENCE - Inheritence states that creation of a new class by making use of existing class
>It can be defined as deriving a child class inheriting features of parent class.
________________________________
>>>>>>>>SUPER CLASS/PARENT CLASS   
           |
           |
>>>>>DERIVED CLASS/CHILD CLASS      
_________________________________
public class A
{
....
}
public class B extends A
{
...
}
#SYNTAX
class parent-class_name
{
  private/public/protected data members
     member functions
}
class child_class_name extends parent_class_name
{
 private/public/protected data members
   member functions
}
#EXAMPLE 3.1:
class Student
{
  int id;// data member
}
class Stu_details extends Student
{
 // member function
 void display()
 {
 System.out.println(id);
 }
}
Example 3.2:
//childclass
package inheritenceExample;
public class Student {
  int id;
}
//parentclass
package inheritenceExample;
public class StuDwtails extends Student {
 String Name; //data member
 void display()
 {
   System.out.print(id+"|"+Name);
  }
  package inheritenceExample;
  public class Basic {
    public static void main(String args[]) {

      StuDetails obj=new StuDetails();//object of child class
      obj.id=123;
      obj.Name="John";
      obj.display();
      O/P:123|John
>>>POLYMORPHISM<<<<
>Existing in many forms is polymorphism
>>Poly - MANY &  morphism - FORMS

        P    O  L  Y  M  O  R  P  H  I  S  M
        |                  
    COMPILE time/Static           RUNTIME / Dynamic
     |                                   |
     Overloading                   Overriding
Method Overloading
Method with same name existing multiple times in same class but with different type of PARAMETERS
                |    Student           |
                |       |              |
                | print(marks1,marks2) |
                |       |              |
                | print(id,name)       |
                |       |              | 
                | print(grade)         |
#Syntax
class parent_class_name
{
  Returntype1 Function_A(Parameter1)
  {Def1}
  Returntype2 Function_A(P1,P2)
  {Def2}
  Returntype2 Function_A(P1,P2,P3)
  {Def2}
  }
  
  Example-4.1
  class Shape
  {
   void draw9height,width)
   { ......
     System.out.println(draw rectangle);
     }
     void draw(radius)
     {
        System.out.println(draw circle);
     }
     void draw(side)
     {
        System.out.println(draw square);
     }
    }

    
>>>Method Overriding<<<
#In INHERITENCE, when child class redefines METHOD of parent class,it is called METHOD OVERRIDING.
>>>Note- The member FUNCTION PROTOTYPE or SIGNATURE must be same in child and parent class.

                          s--------->     Draw() Circle
                         Shape ---------> Draw() rectangle
                          s---------->    Draw() square
                         Draw()
Example:4.2
package oop.Example;
public class Student {
  void addMarks(int a,int b)
  {
      System.out.println(Adding 2 integers " +a +" + " +b"+ : "+(a+b));
  }
  void addMarks(int a)
  {
      System.out.println(Adding integer " + a + " to 500 " + (a+500));
  }
  void addMark(float a,float b,float c)
  { 
       System.out.println("Adding 3 floats " + (a+b+c));
   }
 } 

 <<<<<<<
 package opp.Example;

 public class Basic {

 Student obj=new Student();//object of Student class
 obj.addMarks(75,85);
 obj.addMarks(98);
 obj.addMarks(75.456f, 85.457f, 98.658f);
 O/P:
 Adding 2 integers 75+85: 160
 Adding integer 98 to 500 598
 Adding 3 floats 259.57098

 >>>
> >>package oop.Example;
public class StuDetails extends Student {
    void addMarks(int a,int b)
    {
      System.out.println("Adding 2 integers to 1000" +a +" + " +b+": "+(a+b+1000));
    }
}
 
>>>>Method OVERRIDING<<<<
>>In INHERITENCE, when child class redefines METHOD of parent class, it is called METHOD OVERIDING.
>>>>Note- The member FUNCTION PROTOTYPE or SIGNATURE must be same in child and parent class.
#SYNTAX
class parent_class_name
{
  Returntype Function1()
  {Defined}
}
class child_class_name extends parent_class_name
{
   Returntype Function1()
   {Re Defined/Overriden}
Example: 4.1.1
 class Shape
 {
  void draw()
  {
    System.out.println(draw shape);
  }
}
class Triangle extends Shape
{
  // member function
     void draw()
     {
          System.out.println(draw triangle);
     }
}
>>>>ABSTRACTION<<<<<
>>Hiding functionality/implementation and showing only necessary details is Abstraction.
>>>>Note: ABSTRACT CLASS and INTERFACES are used to acheive ABSTRACTION in java.
_________________
Employee       >>>>..>>>>>   Teacher DisplayDetails()
DisplayDetails() >>>>>>>>     Accountant DiplayDetails()
__________________>>>>..>...>.> Principal DisplayDetails()





















 
 

                         
                         
               
  






  
























































