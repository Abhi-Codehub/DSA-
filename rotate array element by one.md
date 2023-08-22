# Rotate Array Element by one
```
class Compute {
    
    public void rotate(int arr[], int n){
       
       int last = arr[n-1];
       
       for(int i = n-1; i>0; i--){
           arr[i] = arr[i-1];
       }
       arr[0] = last;
    }
}
```
<img width="419" alt="Screenshot 2023-08-22 at 11 36 57 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/d415fec1-b753-4c8d-8f3d-56bf84777e1e">

