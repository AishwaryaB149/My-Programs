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



//In an array of numbers just sort the even numbers in the array and donot change the position of odd numbers
import java.util.*;
class OddStableSort
{
	public static void main(String[] args)
	{
		int evenCounter=0;		
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the n value: ");
		int n=sc.nextInt();
		int[] arr=new int[n];
		System.out.println("Enter "+n+" numbers: ");
		for(int i=0;i<n;i++)
		{
			arr[i]=sc.nextInt();
			if(arr[i]%2==0)
			{
				evenCounter++;
		      }
		}
		int [] b=new int[evenCounter];
		int j=0;
		for(int i=0;i<n;i++)
		{
			if(arr[i]%2==0)
			{
				b[j]=arr[i];
				j++;
			}
		}
		Arrays.sort(b);
		j=0;
		System.out.println("Result= ");
		for(int i=0;i<n;i++)
		{
			if(arr[i]%2==0)
			{
				arr[i]=b[j];
				j++;
			}
		      System.out.printf("%4d",arr[i]);
		}
	}
}
//another approach

import java.util.*;
class OddStableSort
{
	public void sortEvenNumbersOnly(int[] arr)
	{
		int[] evens=Arrays.stream(arr).filter(x -> x%2==0).sorted().toArray();
	      int j=0;
		for(int i=0;i<arr.length;i++)
		{
			if(arr[i]%2==0)
			{
				arr[i]=evens[j++];
			}
		}	 
	}
	public static void main(String[] args)
	{
		OddStableSort obj=new OddStableSort();
		int[] arr={25,34,28,44,9,27,13,6};
		System.out.println("Original array: "+Arrays.toString(arr));
		obj.sortEvenNumbersOnly(arr);
		System.out.println("Sorting even numbers: "+Arrays.toString(arr));
	}

}





