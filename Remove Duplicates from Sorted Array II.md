#Remove Duplicates from Sorted Array II
```
class Solution {
    public int removeDuplicates(int[] nums) {

        int x = 2;
        for(int i = x; i<nums.length; i++){
            if(nums[i] != nums[x-2]){
                nums[x++] = nums[i];
            }
        }
        return x;
    }
}
```
<img width="843" alt="Screenshot 2023-06-12 at 10 00 30 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/ee07fd28-753b-4866-89d6-381f1389391d">
