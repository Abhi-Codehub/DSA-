# Contains Duplicate
```
class Solution {
    public boolean containsDuplicate(int[] nums) {
     for (int i=0; i<nums.length; i++){
            for (int j=i+1; j<nums.length; j++){
                if(nums[i] == nums[j]){
                    return true;
                }
            }
        }
     return false;
  }
}  
   
```
```
class Solution {
public boolean containsDuplicate(int[] nums) {
 Arrays.sort(nums);
    int a = nums[0];
    for(int i = 1; i<nums.length; i++){
        if(nums[i]!= a){
            a = nums[i];     
        } 
        else {
            return true;
        }
    }
    return false;

    }
}
```
<img width="788" alt="Screenshot 2023-08-03 at 5 13 08 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/933c7983-5428-41d0-bd92-ff366b33a171">

