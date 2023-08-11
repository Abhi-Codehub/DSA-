# Remove Consecutive Characters
```
class Solution{
    public String removeConsecutiveCharacter(String S){
        
        String str = "";
        char ch = S.charAt(0);
        str = str + ch;
        int i = 1;
        while(i < S.length()){
            if(S.charAt(i) != S.charAt(i-1)){
                str += S.charAt(i); 
            }
            i++;
        }
        return str;
    }
}
```
<img width="390" alt="Screenshot 2023-08-11 at 2 29 50 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/548f81ca-f248-4b1d-a860-6b132fde74c1">
