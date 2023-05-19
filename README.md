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
