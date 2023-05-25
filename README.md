# ARRAYQUESTION

1. SPAN OF ARRAY 


       Scanner p=new Scanner(System.in);
         int n=p.nextInt();
         int []arr=new int[n];
         
         for(int i=0;i<n.length;i++)
         {
             arr[i]=p.nextInt();
             
         }
        
        int max=arr[0];
        int min=arr[0];
         for(int i=1;i<n.length;i++)
         {
            if(arr[i]>max)
            {
                max=arr[i];
            }
            if(arr[i]<min)
            {
                min=arr[i];
            }
            
         }
         
         int span=max-min;
         System.out.println(span);
     }
     
2. find the element 
     
          public static void main(String[] args) 
          {
     
          Scanner s=new Scanner(System.in);
           int n=s.nextInt();
      
           int[] arr=new int[n];
      
            for(int i=0;i<arr.length;i++)
            {
             arr[i]=s.nextInt();
             }
      
     
            int match=s.nextInt();
            int index=-1;
           for(int i=0;i<arr.length;i++)
           {
            if(arr[i]==match)
           {
             index=i;
             break;
           }
        
         }
            System.out.println(index);
      
  }
  
3.BAR CHART


   public class Main
    {
    
    
     public static void main(String[] args) {
      
      Scanner s=new Scanner(System.in);
      int n=s.nextInt();
      
      int[] arr=new int[n];
      
      for(int i=0;i<arr.length;i++)
      {
        arr[i]=s.nextInt();
      }
      
     
       int max=arr[0];
      for(int i=1;i<arr.length;i++)
      {
        if(arr[i]>max)
        {
          max=arr[i];
        }
        
      }
      
      for(int floor=max;floor>=1;floor--)
      {
        for(int i=0;i<arr.length;i++)
        {
          if(arr[i]>=floor)
          {
            System.out.println("*\t");
          }
          else
          {
            System.out.println("\t");
          }
        }
      System.out.println();
       }
      
    }
}
  
3.SUM OF 2 ARRAY
          
          
          
          public static void main(String[] args) {
      
      Scanner s=new Scanner(System.in);
      int n=s.nextInt();
      
      int []arr1=new int[n];
      for(int i=0;i<arr1.length;i++)
      {
        arr1[i]=s.nextInt();
      }
      
      int m=s.nextInt();
      
      int []arr2=new int[m];
      for(int i=0;i<arr2.length;i++)
      {
        arr1[i]=s.nextInt();
      }
      
      int []sum=new int[n>m?n:m];
      int c=0;
      
      int i=arr1.length-1;
      int j=arr2.length-1;
      int k=sum.length-1;
      
      while(k>=0)
      {
        int d=c;
        if(i>=0)
        {
          d+=arr1[i];
        }
        if(j>=0)
        {
          d+=arr2[j];
          
        }
        c=d/10;
        d=d%10;
        sum[k]=d;
        
        i--;
        j--;
        k--;
        
        
        
      }
      if(c!=0){
        System.out.println(c);
      }
      for(int val:sum)
      {
        System.out.println(val);
      }
 
 
 
 REVERSE AN ARRAY
 
 
      
      
      public class Main {
    public static void main(String[] args) {
      
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      int []arr=new int[n];
      
      for(int i=0;i<arr.length;i++)
      {
        arr[i]=s.nextInt();
      }
      
      for(int j=arr.length-1;j>=0;j--)
      {
        System.out.println(arr[j]);
      }
   
   
   
IS PRIME USING ARRAY




       public static void main(String[] args) throws Exception
    {
    
    Scanner s=new Scanner(System.in);
    int n=s.nextInt();
    
  
     int[]arr=new int[n];
     for(int i=0;i<arr.length;i++)
     {
       arr[i]=s.nextInt();
     }
       
     for(int i=0;i<arr.length;i++)
     {
       int count=0;
       for(int j=1;j<=arr[i];j++)
       {
         if(arr[i]%j==0)
         {
           count++;
         }
       }
       if(count==2)
       {
         System.out.println("Prime no."+arr[i]);
       }
       else
       {
         System.out.println("not prime :"+arr[i]);
       }
     }
  }
}
   
   
   
   
   
FIBONACI SERIES


        
        
    public static void main(String[] args) throws Exception
    {
    
    Scanner s=new Scanner(System.in);
    int P=s.nextInt();
    
      int n1=0;
      int n2=1;
      
     
     for(int i=0;i<P;i++)
     {
       System.out.println(n1);
       int c=n1+n2;
       n1=n2;
       n2=c;
       
     }
    }
  
};
   


COUNT THE DIGITS OG NUMBER


      
      public static void main(String[] args) {
      
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      
      int count=0;
      while(n!=0)
      {
        n=n/10;
        count++;
      }
      System.out.println(count);
  }




Print the count number from left to right




       public static void main(String[] args) {
      
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      
      int count=0;
      int temp=n;
      while(temp != 0)
      {
        temp=temp/10;
        count++;
      }
      int div=(int)Math.pow(10,count-1);
      
      while(n != 0)
      {
        int q=n/div;
        System.out.println(q);
        
        n=n%div;
        div=div/10;
      }
      }
      
      
      
      
      
  REVERSE A NUMBER
  
  
  
      public static void main(String[] args) {
      
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      
     while(n!=0)
     {
       int q=n%10;
       System.out.println(q);
       n=n/10;
     }
     }
