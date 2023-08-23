# find the sum of max and min of an array 
```
class Solution
{ 
    public static int findSum(int A[],int N) 
    {
        //code here
        int max = A[0];
        int min = A[0];
        for(int i = 1; i<N; i++){
            if(A[i] > max){
                max = A[i];
            }
            if(A[i] < min){
                min = A[i];
            }
        }
        int sum = max+min;
        return sum;
    }
}

```
<img width="517" alt="Screenshot 2023-08-23 at 1 45 16 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/46215014-677c-4dde-b542-2afd373e5cd2">

