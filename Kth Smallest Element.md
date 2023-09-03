# kth Smallest Element 
```
class Solution{
    public static int kthSmallest(int[] arr, int l, int r, int k) 
    { 
       // Solving this problem using Heaps Maxheap 
       
       int n = arr.length;
       
       PriorityQueue<Integer> minH = new PriorityQueue<>((a,b) -> b - a);
       
       for(int i = 0; i<n; i++){
           minH.add(arr[i]);
           
           if(minH.size() > k){
               minH.remove();
           }
       }
       return minH.peek();
    } 
}
```
<img width="459" alt="Screenshot 2023-09-03 at 3 55 51 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/c5c78712-2f1a-42eb-a78c-88bb6fc8375e">

