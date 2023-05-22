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
    }
  }
