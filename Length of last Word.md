# Length of last Word
```
class Solution {
    public int lengthOfLastWord(String s) {
        
        int length = 0;
        for (int i = s.length()-1; i>=0; i--){
            if(s.charAt(i)!= ' '){
                length++;
            }
            else{
                if(length>0)
                return length;
            }
        } 
        return length;
    }
}
```
<img width="766" alt="Screenshot 2023-06-14 at 10 37 52 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/866dfdac-c33d-48a9-bbf4-67df9b999181">


