# Next Permutation 
```
class Solution {
    public void nextPermutation(int[] nums) {

        int index1 = -1;
        int index2 = -1;
        int n = nums.length;

        for(int i = n-2; i>=0; i--){
            if(nums[i] < nums[i+1]){
                index1 = i;
                break;
            }
        }
        if (index1 == -1){
           Arrays.sort(nums);
            }
        else {
            for(int i=n-1; i>=0; i--){
                if(nums[i] > nums[index1]){
                    index2 = i;
                    break;
                }
            }
            swap(nums, index1, index2);
            reverse(nums, index1+1);
        }
    }
        void swap (int[] nums, int i, int j){
            int temp = nums[i];
            nums[i] = nums[j];
            nums[j] = temp;
        }    
        void reverse(int [] nums, int start){
            int i = start;
            int j = nums.length-1;
            while(i<j){
                swap(nums,i,j);
                i++;
                j--;
            }
        }   
    }
```
<img width="742" alt="Screenshot 2023-08-22 at 7 25 35 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/bd9cc77f-7510-48cd-8a81-28f31a2c87fa">
