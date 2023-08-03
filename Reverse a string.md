# Reverse a String 
```
class Reverse
{
    // Complete the function
    // str: input string
    public static String reverseWord(String str)

    {
        int x = str.length();
        String reverse = "" ;
            
        for (int i = x-1; i>=0; i--){
            reverse = reverse + str.charAt(i); 
            
        }
        
       return reverse;
    }
}
```
<img width="428" alt="Screenshot 2023-08-03 at 2 25 22 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/df394638-6fb6-4d21-be23-779672151062">
