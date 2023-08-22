# Union of Arrays
```
class Solution{
    public static int doUnion(int a[], int n, int b[], int m) 
    {
        int count1 = 0;
        HashSet<Integer> set = new HashSet<>();
        for(int i=0; i<n; i++){
            if(!set.contains(a[i]) ){
                set.add(a[i]);
                count1++;
            }
        }
        int count2 = 0;
        for(int i=0; i<m; i++){
            if(!set.contains(b[i])){
                set.add(b[i]);
                count2++;
            }
        }
        int result = count1+count2;
        return result;
    }
}
```
<img width="467" alt="Screenshot 2023-08-22 at 10 29 43 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/ea832ca1-2273-444e-90bf-0daed1ffef6c">
