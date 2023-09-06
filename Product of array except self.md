# Product of an Array except self
```
class Solution {
    public int[] productExceptSelf(int[] nums) {
        
        int n = nums.length;
        int product = 1;

        int [] result = new int[n];
        int [] left_pro = new int[n];
        int[] right_pro = new int[n];

        right_pro[n-1] = 1;
        left_pro[0] = 1;

        for(int i = 1; i<n; i++){
            left_pro[i] = nums[i-1] * left_pro[i-1];
        }

        for(int i = n-2; i>=0; i--){
            right_pro[i] = nums[i+1] * right_pro[i+1];
        }
        for(int i = 0; i < n; i++){
        result[i] = left_pro[i] * right_pro[i];
        }
        return result;
    }

}

```
<img width="723" alt="Screenshot 2023-09-06 at 4 03 25 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/308f666e-55db-4838-8cb0-d722ef7f9bbf">

