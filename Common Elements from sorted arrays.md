# Common Elements From Sorted Arrays
```
class Solution
{
    ArrayList<Integer> commonElements(int A[], int B[], int C[], int n1, int n2, int n3) 
    {
        ArrayList<Integer> commonElements = new ArrayList<>();

       int i = 0, j = 0, k = 0;
       while(i<n1 && j<n2 && k<n3){
           if(A[i] == B[j] && B[j] == C[k]){
               if(!commonElements.contains(A[i]))
              commonElements.add(A[i]);
            i++;
            j++;
            k++;
           }
            else if (A[i] < B[j]){
                    i++;
            } 
            else if (B[j] < C[k]){
                    j++;
            }
            else 
                    k++;
            }
            return commonElements;
    }
}
```
<img width="485" alt="Screenshot 2023-08-08 at 8 22 17 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/de1a5173-80cc-4b94-bc61-9a9fe72438d9">


