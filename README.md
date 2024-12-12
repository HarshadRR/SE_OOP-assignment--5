# SE_OOP-assignment--5 [ Design and develop a context for given case study and implement an interface for Vehicles Consider
the example of vehicles like bicycle, car and bike. All Vehicles have common functionalities such as
Gear Change, Speed up and apply breaks. Make an interface and put all these common functionalities. Bicycle, Bike, Car classes should be implemented for all these functionalities in their own class in their
own way.]





import java.util.*;
interface Vehicles
{
void speedUp();
void applyBreaks();
void gearChange();
}
class Bycicle implements Vehicles{
public void gearChange()
{
Scanner sc=new Scanner(System.in);
System.out.println("Enter Gear :");
int a=sc.nextInt();
if(a!=0)
{
a++;
}
System.out.println("Gear changed of Bycicle:" + a);
}
public void speedUp(){
Scanner sc=new Scanner(System.in);
System.out.println("Enter speed :");
int a=sc.nextInt();
if(a!=50)
}

a=a+10;
}
System.out.println("Speed of Bycicle is changed to :" + a);
}
public void applyBreaks(){
System.out.println("Applied breaks of Bycicle");
}
}
class Bike implements Vehicles{
public void gearChange()
{
Scanner sc=new Scanner(System.in);
System.out.println("Enter Gear :");
int a=sc.nextInt();
if(a!=0)
{
a++;
}
System.out.println("Gear changed of Bike to :" +a);
}
public void speedUp(){
Scanner sc=new Scanner(System.in);
System.out.println("Enter speed :");
int a=sc.nextInt();
if(a!=50)
{
a=a+10;
}
System.out.println("Speed of Bike is changed to:"+a);
}
public void applyBreaks(){
System.out.println("Applied breaks of Bike");
}
}
class Car implements Vehicles{
public void gearChange()
{
Scanner sc=new Scanner(System.in);
System.out.println("Enter Gear :");
int a=sc.nextInt();
if(a!=0)
{
a++;
}
System.out.println("Gear changed of Car:" +a);
}
public void speedUp(){
Scanner sc=new Scanner(System.in);
System.out.println("Enter speed :");
int a=sc.nextInt();
if(a!=50)
{
a=a+10;
}
System.out.println("Speed of Car is changed to:"+a);
}
public void applyBreaks(){
System.out.println("Applied breaks of Car");
}
}
class Interfaces
{
public static void main(String[] args) {
Vehicles v;
v= new Bycicle();
System.out.println("--Bycicle--");
v.gearChange();
v.speedUp();
v.applyBreaks();
v= new Bike();
System.out.println("--Bike--");
v.gearChange();
v.speedUp();
v.applyBreaks();
v= new Car();
System.out.println("--Car--");
v.gearChange();
v.speedUp();
v.applyBreaks();
}
}
