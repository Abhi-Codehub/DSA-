# Valid Palindrome
```
class Solution {
    public boolean isPalindrome(String s) {
        if(s.isEmpty()){
            return true;
        }
        int start = 0;
        int last = s.length()-1;
        while (start<=last){
            char currFirst = s.charAt(start);
            char currLast = s.charAt(last);
            if(!Character.isLetterOrDigit(currFirst)){
                start++;
            }
            else if(!Character.isLetterOrDigit(currLast)){
                last--;
            }
            else { if(Character.toLowerCase(currFirst)!= Character.toLowerCase(currLast)) {
                    return false;
                    }
                start++;
                last--;
            }
        }
        return true;  
    }
}
```
<img width="770" alt="Screenshot 2023-06-17 at 12 07 11 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/2e0de139-c89a-4a46-928d-c982bd86dc0a">



