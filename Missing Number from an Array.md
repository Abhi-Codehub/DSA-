# Missing Element from an Array 
```
class Solution {
    int MissingNumber(int array[], int n) {
        // Your Code Here
        int sum =0;
        for (int i=0; i<array.length; i++){
            sum = sum+array[i];
        }
        int tSum = ( n * (n+1)) / 2;
        return tSum-sum;
    }
}
```
<img width="503" alt="Screenshot 2023-04-17 at 10 44 33 PM" src="https://user-images.githubusercontent.com/111800760/232561188-f71e3243-843c-4e3e-99c9-7bb2dbd2681f.png">

