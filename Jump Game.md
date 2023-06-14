# Jump Game
```
class Solution {
    public boolean canJump(int[] nums) {

        int n = nums.length;
        int reachable = 0;
        for(int i = 0; i<n; i++){
            if(reachable < i){
                return false;
            }
            else 
            reachable = Math.max(reachable, i+nums[i]);
        }
        return true; 
    }
}
```

<img width="776" alt="Screenshot 2023-06-14 at 11 24 13 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/04314d4d-a10d-4c6b-b588-b2cc0aeb254d">

