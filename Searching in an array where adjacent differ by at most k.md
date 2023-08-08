# Searching in an array where adjacent differ by at most k
```
class Complete{
   
    // Function for finding maximum and value pair
    public static int search (int arr[], int n, int x, int k) {
        for(int i = 0; i<arr.length; i++){
            if(arr[i] == x){
                return i;
            }
        }
        return -1;
        
    }
}
```
<img width="428" alt="Screenshot 2023-08-08 at 11 40 51 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/47e1a8ec-669d-47f9-9530-e6ffce6c9075">

