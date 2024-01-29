# practice-question
# Question 1:-
import java.util.*;
class Main {
  public static void main(String[] args) {
     
Scanner sc = new Scanner(System.in);
    int n=sc.nextInt();
      int a = 0;
    int b = 1;
    System.out.println("Fibonacci Series till " + n + " terms:");

    for (int i = 1; i <= n; ++i) {
      System.out.print(a+" " );
      int c = a + b;
      a = b;
b = c;
    }
  }
}

# Question 2:-
import java.util.*;
class Main { 
  public static void main(String[] args) 
  {
      int x;
      int  sum = 0;
      float average;
      Scanner s = new Scanner(System.in);
      System.out.print("Enter x");
      x = s.nextInt();
      int a[] = new int[x];
      System.out.println("input numbers");
      for(int i = 0; i < x ; i++)
      {
          a[i] = s.nextInt();
          sum = sum + a[i];
      }
      average = sum / x;
      System.out.println("Average:"+average);
  }
 }
 
# Question 3:-
class Vehicle{
public String make;
public String model;
public int year;
   
}
class Car extends Vehicle {
 public String fuelType;
   Car(){
     System.out.println("Car is created");
   }   
  void Show(String fuelType,String make,String model,int year){
    this.fuelType = fuelType;
    this.make=make;
    this.model=model;
    this.year=year;
  }
}


public class Main {
  public static void main(String[] args) {
    Car car = new Car();
    car.Show("diesel","Toyota","Camry",2020);
    System.out.println(car.fuelType);
    System.out.println(car.make);
    System.out.println(car.model);
    System.out.println(car.year);
    
       
  }
}

# Question 4:-
import java.util.*;

class Rectangle {

  
  void Area(int length, int width)
  {
    double area;
    area = length *width;
    System.out.println("Area of rectangle is : "+ area);
  }

  void Perimeter(int length, int width)
  {
    double perimeter;
    perimeter = 2 * (length +width);
    System.out.println("Perimeter of rectangle is : "+ perimeter);
  }
}
  class Circle {

  void Area( int radius)
  {
    double area;
    area = 3.14 *radius*radius;
    System.out.println("Area of rectangle is : "+ area);
  }

 
    void Perimeter(int radius)
    {
     double perimeter;
      perimeter = 2 * 3.14 * radius;
      System.out.println("Perimeter of rectangle is : "+perimeter);
    }
}

class Main {

  public static void main(String args[]){
    Rectangle o = new Rectangle();
    o.Area(2,3);
    o.Perimeter(2,3);
    Circle c = new Circle();
    c.Area(2);
    c.Perimeter(2);
    
  }
}

# Question 5:-
interface Drawable{
  void draw();

}

abstract class Shape implements Drawable{
public void draw(){
  System.out.println("Drawing...");
}
}

 class Square implements Drawable{
  public void draw(){
    System.out.println("Drawing Square...");
  }
  
}

 class Circle implements Drawable{
    public void draw(){
      System.out.println("Drawing Circle...");
    }

}


class Main {
  public static void main(String[] args) {
    Drawable d1 = new Square();
    d1.draw();
    Drawable d2 = new Circle();
    d2.draw();
    
  }
}
