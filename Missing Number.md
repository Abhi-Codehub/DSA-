# Missing Number from an array
```
class Solution {
    public int missingNumber(int[] nums) {

        int n = nums.length;
        int maxSum = (n * (n+1)) / 2;
        int sum = 0;

        for(int i =0; i<n; i++){
            sum += nums[i];
        }
        return maxSum-sum;
    }
}
```
<img width="751" alt="Screenshot 2023-08-23 at 12 06 46 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/ecdfb666-2c76-404a-bc15-d922bacabea7">
