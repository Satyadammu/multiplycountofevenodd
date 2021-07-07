# multiplycountofevenodd
import java.util.*;
public class Even_Odd
{
    public static void main(String[] args) 
    {
        int n,res;
        int count_odd=0;
        int count_even=0;
        Scanner s = new Scanner(System.in);
        System.out.print("Enter size of elements:");
        n = s.nextInt();
        int a[] = new int[n];
        System.out.println("Enter all the elements:");
        for (int i = 0; i < n; i++) 
        {
            a[i] = s.nextInt();
        }
        for(int i = 0 ; i < n ; i++)
        {
            if(a[i] % 2 != 0)
            {
              count_odd++;
            }
        }
        for(int i = 0 ; i < n ; i++)
        {
            if(a[i] % 2 == 0)
            {
              count_even++;
            }
        }
        res=count_odd*count_even;
        System.out.println("product of even and odd no of elements"+res);
        if(res%2==0)
        System.out.println("result is an even number");
        else
        System.out.println("result is an odd number");
        
        
    }
}
