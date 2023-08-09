# Find a pair with the given difference
```
class Solution {

    public boolean findPair(int[] arr, int size, int n) {
        Arrays.sort(arr);
        int i = 0;
        int j = 1;
        while (i < size && j < size) {
            if (i != j && ((arr[j] - arr[i] == n) || (arr[i] - arr[j] == n))) {
                return true;
            } else if (arr[j] - arr[i] < n) {
                j++;
            } else {
                i++;
            }
        }
        return false;
    }
}
```
<img width="499" alt="Screenshot 2023-08-09 at 3 38 43 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/0745e354-4d3c-46c9-99ba-94e1d835900d">
