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
