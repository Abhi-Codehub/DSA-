# Rotate an Array by kth Element 

```
class Solution {

    public static void reverse (int[] nums, int start, int end){
        while(start < end){
            int temp = nums[start];
            nums[start] = nums[end];
            nums[end] = temp;
            start++;
            end--;
        }
    }
    public void rotate(int[] nums, int k) {
        k %= nums.length;
        reverse (nums, 0, nums.length -1 );
        reverse (nums, 0, k-1);
        reverse (nums, k, nums.length-1);
    }
}
```
<img width="782" alt="Screenshot 2023-06-13 at 7 34 00 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/8580c6a1-e468-4f02-8dee-a83bb21a81e5">


