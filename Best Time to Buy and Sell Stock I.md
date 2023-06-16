# Best Time to Buy and Sell Stock
```
class Solution {
    public int maxProfit(int[] prices) {
        int lsf = Integer.MAX_VALUE; // least so far 
        int op = 0; // overall price 
        int pist = 0; // profit if sold today
        
        for (int i = 0; i< prices.length; i++){
            if( prices[i] < lsf){
                lsf = prices[i];
            }
            pist = prices[i] - lsf;
            if(op< pist){
                op = pist ;
            }
        }
        return op;
    }
}
```
