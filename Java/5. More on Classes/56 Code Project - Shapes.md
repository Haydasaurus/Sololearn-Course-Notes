# Shapes
You are working on a graphical app, which includes multiple different shapes.  
The given code declares a base **Shape** class with an abstract **area**() method and a **width** attribute.  
You need to create two **Shape** subclasses, **Square** and **Circle**, which initialize the width attribute using their constructor, and define their **area**() methods.  
The **area**() for the **Square** class should output the area of the square (the square of the width), while for the **Circle**, it should output the area of the given circle (PI*width*width).  
The code in main creates two objects with the given user input and calls the area() methods.  
  
**Sample Input:**  
5  
2  
  
**Sample Output:**  
25  
12.566370614359172  
  
The area of the square is 5*5=**25**, while the area of the circle is PI*2*2=**12.566370614359172**  

Use the **Math.PI** constant for the area calculation of the circle.

```java
import java.util.Scanner;

abstract class Shape {
    int width;
    abstract void area();
    double k = Math.PI;
    int width1;
    double width2;
}

//your code goes here

class Square extends Shape{

public Square (int width){
	this.width = width;
}
void area (){
int width1= (width*width);
System.out.println (width1);
}
	
}
class Circle extends Shape{
public Circle (int width){
	this.width = width;
}
void area(){
	double width2 = ((k)*width*width);
	System.out.println (width2);
}

}
public class Program {
    public static void main(String[ ] args) {
        Scanner sc = new Scanner(System.in);
        int x = sc.nextInt();
        int y = sc.nextInt();
        
        Square a = new Square(x);
        Circle b = new Circle(y);
        a.area();
        b.area();
    }
}
```