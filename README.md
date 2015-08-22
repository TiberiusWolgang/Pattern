# Pattern
//Increasing/Decreasing spaces pattern

import java.util.Scanner;
public class bhiPeetaHai {
	
	public static void main(String[] args){
		
		Scanner s = new Scanner(System.in);
		System.out.print("Enter the length of the pattern: ");
		int k = s.nextInt();
		int i, j, max=k, tot=1, a, b, tot1=1, max1=k-1;
		for(b=1; b<=2; ++b)
		{
			if(b==1)
			{
				for(a=1; a<=k; ++a)
				{
					for(i=1; i<=max; ++i)
					{
						System.out.print(" ");
					}
					--max;
					
					for(j=1; j<=tot; ++j)
					{
						System.out.print("X ");			
					}
					++tot;
					System.out.println("");
					}
				}
			
			else if(b==2)
			{
				for(a=1; a<=k-1; ++a)
				{
					for(i=0; i<=tot1; ++i)
					{
						System.out.print(" ");
					}
					++tot1;
					
					for(j=1; j<=max1; ++j)
					{
						System.out.print("X ");			
					}
					--max1;
					System.out.println("");
					}
			}
		}
	}
}
