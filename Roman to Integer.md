# Roman to Integer
```
class Solution {
    public int romanToInt(String s) {

        int ans = 0;
        int number = 0;
        int prev =0;

        for(int i=s.length()-1; i>=0; i--){
            switch(s.charAt(i)){
                case 'I' -> number =  1;
                case 'V' -> number =  5;
                case 'X' -> number =  10;
                case 'L' -> number =  50;
                case 'C' -> number =  100;
                case 'D' -> number =  500;
                case 'M' -> number =  1000;
            }
            if(number < prev){
                ans -= number; 
            }
            else {
                ans+= number;
            }
            prev = number;
        }
        return ans;
    }
}
```
<img width="774" alt="Screenshot 2023-06-17 at 4 36 35 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/82a7cb06-f1b5-4a67-b31f-4cb6bd198534">

