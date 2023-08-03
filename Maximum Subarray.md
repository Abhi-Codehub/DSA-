# Maximum Subarray 
```
class Solution {
    public int maxSubArray(int[] nums) {
        int currsum = 0; 
        int maxsum = Integer.MIN_VALUE;

        for(int i =0; i<nums.length; i++){
            currsum += nums[i]; 
            if(currsum > maxsum){
                maxsum = currsum;
            }
            if(currsum<0)
            currsum = 0;
        }
        return maxsum;
        
    }
}
```
<img width="750" alt="Screenshot 2023-08-03 at 3 54 42 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/28f277b9-1052-499c-be69-d882e81b6057">
