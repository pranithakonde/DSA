# Snapchat
import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		Scanner s = new Scanner(System.in);
		int t = s.nextInt();
		
		for(int i=0;i<t;i++)
		{
		    int n = s.nextInt();
		    int count=0,max=0;
		    int[] a=new int[n];
		    int[] b=new int[n];
		    for(int j=0;j<n;j++)
		    {
		         a[j]=s.nextInt();
		    } 
		    for(int k=0;k<n;k++)
		    {
		         b[k]=s.nextInt();
		    }
		    for(int l=0;l<n;l++)
		    {
		        if((b[l]==0)||(a[l]==0))
		            count=0;
		            
		        else
		            count++;
		            if(count>max)
		                max=count;
		    }
		    System.out.println(max);
		}
	}
}
