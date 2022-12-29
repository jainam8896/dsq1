# dsq1

import java.util.*;

public class a3q1 {
    public static void main(String[] args) {
        int a[]={0,1,2,4,6,7,8,9};
        int t = 9;
        System.out.println(search(a,t));
    }
    
    public static int search(int []a,int t)
    {
        int s=0;
        int end = a.length-1;
        while(s<=end)
        {
            int middel =s +(end - s)/2;
            if(a[middel]<t)
            {
                return middel;
            }
            else if(a[middel]<t)
            {
                s = middel+1;
            }
            else if(a[middel]>t)
            {
                end = middel - 1;
            }
        }
        return -1;
    }
}
