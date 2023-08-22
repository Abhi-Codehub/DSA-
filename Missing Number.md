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
