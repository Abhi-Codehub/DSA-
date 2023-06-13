#Majority Element
```
class Solution {
    public int majorityElement(int[] nums) {

        int count = 0; 
        int maxELement = Integer.MIN_VALUE;
        for (int i = 0; i<nums.length; i++){
            if ( count == 0 ){
                maxELement = nums[i];
            }
            if( nums[i] == maxELement){
                count++;
            }
            else {
                count--;
            }
        }
        return maxELement;   
    }
}
```
<img width="762" alt="Screenshot 2023-06-13 at 1 14 09 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/4037a373-055c-44eb-ac18-88a4c7c14f27">
