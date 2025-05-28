# My-Programs
//Find min and max value of given two numbers without using control statements and built in funtions (max() & min())
import java.util.Scanner;
class MinMax
{
	public static void main(String[] args)
	{
		Scanner sc=new Scanner(System.in);
		int a=sc.nextInt();
		int b=sc.nextInt();
		int c=a+b;
		int d=Math.abs(a-b);
		int max=(c+d)/2;
		int min=(c-d)/2;
		System.out.println("Max: "+max);
		System.out.println("Min: "+min);
	}
}


//Find the given number is Even or Odd without using Conditional Statements or Conditional Operator
import java.util.Scanner;
class EvenOdd
{
	public static void main(String[] args)
	{
		Scanner sc=new Scanner(System.in);
		System.out.print("Enter an Integer: ");
		int x=sc.nextInt();
		String[] arr={"Even","Odd"};
		int r =x % 2;
		System.out.println(arr[r]);
	}
}


//Find the sum of two numbers without using Additional Operator
import java.util.Scanner;
class Addition
{
	public static void main(String[] args)
	{
		Scanner sc=new Scanner(System.in);
		System.out.print("Enter a : ");
		int a=sc.nextInt();
		System.out.print("Enter b : ");
		int b=sc.nextInt();
		int s=((a*a)-(b*b))/(a-b);   // int s=a-(-b);
		System.out.println(s);
	}
}


// Find the diff of two numbers without using '-'
import java.util.Scanner;
class Difference
{
	public static void main(String[] args)
	{
		Scanner sc=new Scanner(System.in);
		System.out.print("Enter a : ");
		int a=sc.nextInt();
		System.out.print("Enter b : ");
		int b=sc.nextInt();
		int diff=a+(~b+1);
		System.out.println(diff);
	}
}


//Find the multiplication of two numbers without using '*'
import java.util.Scanner;
class Multiply
{
	public static void main(String[] args)
	{
		Scanner sc=new Scanner(System.in);
		System.out.print("Enter a : ");
		int a=sc.nextInt();
		System.out.print("Enter b : ");
		int b=sc.nextInt();
		int d=int(a/((double)1/b));  //int d=(int)(Math.pow(a+b ,2) - Math.pow(a-b ,2))/4;
		System.out.println(d);
	}
}


