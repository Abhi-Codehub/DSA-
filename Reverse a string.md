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

## Another Approach using byte
```
class Reverse
{
    // Complete the function
    // str: input string
    public static String reverseWord(String str)

    {
       byte[] original = str.getBytes();
       byte[] result = new byte[original.length];
       
       for(int i = 0; i < original.length; i++){
           result[i] = original[original.length -i -1]; 
       }
       return (new String(result));
    }
}
```
<img width="500" alt="Screenshot 2023-08-03 at 3 15 01 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/f62d993e-1d96-4082-ad62-805845bbab69">

