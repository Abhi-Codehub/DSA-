# Is Subsequence
```
class Solution {
    public boolean isSubsequence(String s, String t) {
        int sIndex = 0;
        int tIndex = 0;

        while (sIndex < s.length() && tIndex < t.length()) {
            if (s.charAt(sIndex) == t.charAt(tIndex)) {
                sIndex++;
            }
            tIndex++;
        }
        return sIndex==s.length();
    }
}
```
<img width="906" alt="Screenshot 2023-06-18 at 10 03 05 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/b477a9a7-71ba-4749-a76d-5f9adf4d44ab">

