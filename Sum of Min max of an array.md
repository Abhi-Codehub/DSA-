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

## Second Approach 
``` class Solution
{ 
    public static int findSum(int A[],int N) 
    {
        int max = A[0]; 
        int min = A[0];
        
        for (int i = 0; i<N; i++){
            if(A[i] < min) {
                min = A[i];
            }
            if(A[i] > max){
                max = A[i];
            }
        }
```
<img width="432" alt="Screenshot 2023-08-03 at 1 37 04 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/ae0e8493-1031-4b3f-9954-5d4ae44f4119">

