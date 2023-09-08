# Valid String Palindrome
```
class Solution {
    public boolean validPalindrome(String s) {

        int left = 0;
        int right = s.length() -1 ;

        while(left < right){
            if(s.charAt(left) == s.charAt(right)){
               left++;
               right--;
            }
            else{
                return isPalindrome(s,left+1,right) || isPalindrome(s,left,right-1);
            }
            
        }
        return true;
    }

    public boolean isPalindrome( String s, int left, int right){
        while(left<right){
            if(s.charAt(left) == s.charAt(right)){
               left++;
               right--;
            }
            else {
                return false;
            }
        }
        return true;
    }
}
```
<img width="862" alt="Screenshot 2023-09-08 at 5 08 48 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/49cc72db-99ef-47f4-8873-afd0bdf5ae33">

