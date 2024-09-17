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
Method Overloading_
Method with same name existing multiple times in same class but with different type of PARAMETERS
                |    Student           |
                |       |              |
                | print(marks1,marks2) |
                |       |              |
                | print(id,name)       |
                |       |              | 
                | print(grade)         |
                         
               
  






  
























































