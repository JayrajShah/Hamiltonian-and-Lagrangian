import java.util.*;
public class Hamiltonian {
	
	public static void main(String args[])
	{
		System.out.println("Enter the array size");
		int asize;
		Scanner sc = new Scanner(System.in);
		asize = sc.nextInt();
		int[] arr = new int[asize];
		System.out.println("Enter the array elements");
		for(int i = 0 ; i<asize ; i++)
		{
			arr[i]=sc.nextInt();
		}
		
		for(int i = 0 ; i<asize ; i++)
		{
			if(i!=(asize-1))
			{
				if(arr[i+1]>=arr[i])
				{
					System.out.print("  "+arr[i+1]);
					i++;
				}
			
			}
			else
			{
				System.out.print(" "+arr[i]);
			}
			
		}
		
		
	}

}
