# Sum of Min Max of an array 
```
class Solution
{ 
    public static int findSum(int A[],int N) 
    {
        Arrays.sort(A);
        
        int max = A[0]; 
        int min = A[N-1];
        
    
        int sum = min + max; 
            return sum;
    }
}

```
<img width="535" alt="Screenshot 2023-08-03 at 1 33 28 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/bfcfab61-6391-47e7-b0ca-c24492d81833">
