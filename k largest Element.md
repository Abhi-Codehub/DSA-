# k largest Element 
```
class Solution {
    int[] kLargest(int[] arr, int n, int k) {
        // code here
        
        PriorityQueue<Integer> minH = new PriorityQueue<>();

        for (int i = 0; i < n; i++) {
            minH.add(arr[i]);

            if (minH.size() > k) {
                minH.poll();
            }
        }

        int[] result = new int[minH.size()];
        for (int i = minH.size() -1 ; i >= 0 ; i--) {
            result[i] = minH.poll();
        }

        return result;
    }
}
```
<img width="427" alt="Screenshot 2023-09-03 at 4 44 11 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/ec9aea09-b88f-42ba-b28a-230b28ef53cc">


