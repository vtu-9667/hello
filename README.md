import java.util.*;
import java.lang.*;
public class exercise1 {
    public static void main(String[] args)
    {
        int c=0;
        Scanner n = new Scanner(System.in);
        String A = n.nextLine();
        for(int i=0;i<A.length()-1;i++)
        {
            if((A.charAt(i) !='(' &&  A.charAt(i+1)==')') || (A.charAt(i) !='[' &&  A.charAt(i+1)==']') || (A.charAt(i) !='{' &&  A.charAt(i+1)=='}'))
            {
                c=1;
            }
        }
        if(c==0)
        {
            System.out.println(true);
        }
        else
        {
            System.out.println(false);
        }
    }
}





import java.util.*;
public class exercise1 {
    public static void main(String[] args)
    {
        int c=0,a=0;
        int[] A = new int[]{2,2,1};
        for(int i=0;i<A.length;i++)
        {
            c=0;
            for(int j=0;j<A.length;j++)
            {
                if(A[i] == A[j])
                {
                    c++;
                }
            }
            if(c==1)
            {
                a = A[i];
            }
        }
        System.out.println(a);
    }
}
