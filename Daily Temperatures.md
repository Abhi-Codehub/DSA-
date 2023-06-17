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

