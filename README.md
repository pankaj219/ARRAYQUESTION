# ARRAYQUESTION


GCD AND LCM 


     public class Main {
    public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      int n1=s.nextInt();
      int n2=s.nextInt();
      
      int f1=n1;
      int f2=n2;
      while(n1%n2!=0)
      {
        int rem=n1%n2;
        n1=n2;
        n2=rem;
      }
      int gcd=n2;
      int lcm=(f1*f2)/gcd;
      System.out.println(gcd);
      System.out.println(lcm);
      
     }
    }


CONSECUTIVE ONES (OR ZERO) IN A BINARY ARRAY



      public class Main {
    public static void main(String[] args) {
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      
      int []arr=new int[n];
      for(int i=0;i<arr.length;i++)
      {
        arr[i]=s.nextInt();
      }
      
      
    int count=0;
    for(int i=0;i<arr.length;i++)
    {
      if(arr[i]==1)
      {
        count++;
      }
      else{
        count=0;
      }
    }
    System.out.println(count);
      }
     }


     

MISSING NUMBER FROM THE GIVEN NUMBER


          public class Main {
    public static void main(String[] args) {
      Scanner s =new Scanner(System.in);
      int n=s.nextInt();
      
      int []arr=new int[n];
      for(int i=0;i<arr.length;i++)
      {
        arr[i]=s.nextInt();
      }
      
      
      int xor1=0;
      for(int i=0;i<arr.length;i++)
      {
        xor1=xor1^arr[i];
      }
      
      
      for(int i=1;i<=arr.length+1;i++)
      {
        xor1=xor1^i;
      }
      System.out.println("missing number is :"+xor1);
  }
   }
  







 SPAN OF ARRAY 


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
 
 
 
 ROTATE A NUMBER
 
             
 
        public class Main {
    public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      int n=s.nextInt();
      
      int k=s.nextInt();
      
      int temp=n;
      int nos =0;
      while(temp>0)
      {
         temp=temp/10;
        nos++;
      }
      
      int div=1;
      int mul=1;
      
      for(int i=1;i<=nos;i++)
      {
        if(i<=k)
        {
          div=div*10;
        }
        else{
          mul=mul*10;
        }
      }
      
    int q= n/div;
    int r=n%div;
    
    int ans=r*mul+q;
    System.out.println(ans);
  }
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
   


find the second largest element in array





        public class Main {
    public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      int n=s.nextInt();
      
      int []arr=new int[n];
      for(int i=0;i<arr.length;i++)
      {
        arr[i]=s.nextInt();
      }
      
      int first=Integer.MIN_VALUE;
      int second=Integer.MAX_VALUE;
      
      for(int i=2;i<arr.length;i++)
      {
       
        
        if(arr[i]>first)
        {
          second=first;
          first=arr[i];
        }
        else if(arr[i]<first && arr[i]>second)
        {
          second=arr[i];
        }
      }
      System.out.println(second);
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





STRING






REMOVE WHITE SPACES OF STRING




     
     
       public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      String str=s.nextLine();
      
        char[] strArray = str.toCharArray();  
        StringBuffer stringBuffer = new StringBuffer();  
        for (int i = 0; i < strArray.length; i++) {  
            if ((strArray[i] != ' ') && (strArray[i] != '\t')) {  
                stringBuffer.append(strArray[i]);  
            }  
        }  
        String noSpaceStr2 = stringBuffer.toString();  
        System.out.println(noSpaceStr2);  
       }





REVERSE AN ARRAY



 
 
 
 
       public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      String str=s.nextLine();
      
        char[] strArray = str.toCharArray();  
        StringBuffer stringBuffer = new StringBuffer();  
        
        for(int i=strArray.length-1;i>=0;i--)
        {
          stringBuffer.append(strArray[i]);
        }
        
        String rev=stringBuffer.toString();
        System.out.println(rev);
        }
  


PRINT ALTERNATE CHARATER OF STRING




        public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      String str=s.nextLine();
      
          char []p=str.toCharArray();
          
          StringBuffer br=new StringBuffer();
          
          for(int i=0;i<p.length;i++)
          {
            if(i%2==0)
            {
             br.append(p[i]); 
            }
          }
          String name=br.toString();
          System.out.println(name);
      
      
           }



JAVA STRING





           public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      String present=s.next();
      String next=s.next();
      
      String con=present.concat(next);
      char []name=con.toCharArray();
      
      StringBuffer p=new StringBuffer();
      
      for(int i=name.length-1;i>=0;i--)
      {
        p.append(name[i]);
      }
      String rev=p.toString();
      System.out.println(rev);
      }
      
      
      
      
 FIND CAMEL CASE IN STRING
 
 
 
 
           
           
           public static void main(String[] args) {
      Scanner s=new Scanner(System.in);
      String present=s.next();
      
      char []name=present.toCharArray();
      
      StringBuffer p=new StringBuffer();
      
      for(int i=0;i<name.length;i++)
      {
        if(Character.isUpperCase(name[i]))
        {
           p.append(name[i]);
        }
      }  
      String rev=p.toString();
      System.out.println(rev);
      
    }
    }
    
    
    
    
    
 ALL CHARTER OF STRING IS EQUAL OR NOT 
 
 
 
 
 
      public static void main(String[] args) {
      Scanner s =new Scanner(System.in);
      String str=s.next();
      char []arr=str.toCharArray();
      
      for(int i=0;i<arr.length;i++)
      {
        if(arr[i]==arr[i+1])
        {
          System.out.println("This string is equal:"+true);
          break;
        }
        else
        {
          System.out.println("not equal"+false);
          break;
        }
        }
        
        
        
        
FIND REAPTED CHARATER IN STRING



       public static void main(String[] args) {
      
     Scanner s =new Scanner(System.in);
     String str=s.nextLine();
      
    char []strc=str.toCharArray();
    
    for(int i=0;i<strc.length;i++)
    {
      if(strc[i]==strc[i+1])
      {
        System.out.println(strc[i]+" "+"and index is :"+i);
      }
      }
        
        
        

REPEATED CHARATER 



     public static void main(String[] args) {
      
     Scanner s =new Scanner(System.in);
     String str=s.nextLine();
      
    char []str1=str.toCharArray();
    StringBuffer strbuf=new StringBuffer();
     
     
     for(int i=0;i<str1.length-1;i++)
     {
       for(int j=i+1;j<str1.length;j++)
       {
         if(str1[i]==str1[j])
         {
           strbuf.append(str1[i]);
         }
       }
     }
     
     String ans =strbuf.toString();
     System.out.println(ans);
    }


