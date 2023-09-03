# Kth Largest Element
```
class Solution {
    public int findKthLargest(int[] nums, int k) {

        int n = nums.length;

        PriorityQueue<Integer> maxH = new PriorityQueue<>();

        for(int i = 0; i<n; i++ ){
            maxH.add(nums[i]);
                if(maxH.size() > k){
                    maxH.remove();
                }
        }
        return maxH.peek();
        
    }
}
```
<img width="709" alt="Screenshot 2023-09-03 at 1 05 37 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/89b7242c-f22f-4d80-a3ef-b625b407e1e2">

