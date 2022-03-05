# Java-sum-and-indexing-of-array

import java.util.*;
public class Main
{
  public static void main (String[]args)
  {
    Scanner sc = new Scanner (System.in);
      System.out.println ("Enter the no of elements to be stored in array");
    int n = sc.nextInt ();
int A[] = new int[10];
                                                       
 int sum = 0; 
System.out.println("Enter the elements"); 

    for (int i = 0; i < n; i++)
      {
	A[i] = sc.nextInt ();
      }
      System.out.println("Enter the no to be searched");
      int key = sc.nextInt();
    for (int i = 0; i < n; i++)
      {
	System.out.println(A[i]);
	sum = sum + A[i];
	if(key==A[i]){
	   System.out.println("The index for the elementis :"+i); 
	   System.exit(0);
	}

      }	
      
	System.out.println("Not found:");
      
     
    System.out.println ("The sum for the elements in array is:" + sum);

  }
}
