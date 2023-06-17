#  Daily Temperatures
```
class Solution {
    public int[] dailyTemperatures(int[] temperatures) {

        int length = temperatures.length;
        int [] result = new int[length];
        Stack <Integer> index = new Stack<>();

        for (int i = length -1; i >= 0; i--){
             while(!index.isEmpty() && temperatures[i] >= temperatures[index.peek()])
                index.pop();
        if(!index.isEmpty())
            result[i] = index.peek() - i ;
            index.push(i);
        }
        return result;
    }
}
```
<img width="881" alt="Screenshot 2023-06-17 at 9 01 36 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/29b1241d-53a5-4fbb-93dd-cc5f29134aae">

