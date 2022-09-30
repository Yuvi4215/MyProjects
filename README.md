# MyProjects;
int peakElement(int arr[], int n)

{

    int small = 0;

    int big = n-1;

    int mid = small +(big - small)/2;

    int peak=0;

   while(small<=big)

   {

       if(arr[mid] > arr[mid-1])

       {

           peak = mid;

           small = mid + 1;

       }else{

           big = mid-1;

       }

       mid = small+(big - small) / 2;

   }

   return peak;

}
