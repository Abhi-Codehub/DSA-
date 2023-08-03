# Search In Rotated Array
```class Solution {
    public int search(int[] nums, int target) {
        for(int i = 0; i<nums.length; i++){
            if(nums[i] == target){
                return i;
            }
        }
        return -1;
         }
}
```
<img width="740" alt="Screenshot 2023-08-04 at 12 35 18 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/97f69f67-f2be-474d-9213-65e66a250cb1">
