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

