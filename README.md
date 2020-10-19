# RMT-assignment
import java.util.*;
class RMT
{
	public static void main(String args[])
	{
	
	
		
		Scanner sc = new Scanner(System.in);
		int n = sc.nextInt();
		int ar[] = new int[n];
		for(int i=0;i<n;i++)
		{
			ar[i] = sc.nextInt();
		}
		
		int count = 0;
		HashSet<Integer> set = new HashSet<Integer>();
		for(int i=0;i<n;i++)
		{
			
			int element = ar[i];
			if(set.contains(element))
			{
				set.remove(element);
				count++;
			}
			else
			{
				set.add(element);
			}
			
			
		}
		System.out.println(count);
				
		
    
}
}
