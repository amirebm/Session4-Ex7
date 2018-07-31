
// برنامه ایی بنویسید که پشته را بصورت داینامیک پیاده سازی کند
# Session4-Ex7
package com.personal.Ex7;

import java.util.Scanner;

public class Ex7 {

	static Scanner sc;

	public static void main(String[] args) {

		
		System.out.println("Enter a the size of Stack");
		sc= new Scanner(System.in);
		int arrayLength=sc.nextInt();
		int temp=-1;
		int[] ar= new int[arrayLength];
		
		System.out.println("Please enter "+ arrayLength+ " numbers for Stack:");
		
		for (int i = 0; i < ar.length; i++) {
			
			ar[i]=sc.nextInt();
		}
		printArray(ar);
	    temp=-1;
		while(temp!=0) {
			System.out.println("add new num to the Stack or press 0 to exit");
			ar[ar.length-1]=sc.nextInt();
			temp=ar[ar.length-1];
			printArray(ar);

		}
		System.exit(0);	
		
	}

	static void printArray(int arr[])
	{
	    int n = arr.length;
	    for (int i=0; i<n; ++i)
	        System.out.print(String.format("a[%d]=%d\t", i,arr[i]));
	    System.out.println();
	}
}
