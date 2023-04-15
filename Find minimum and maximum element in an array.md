# Min and Max
```
class Compute 
{
    static pair getMinMax(long a[], long n)  
    {
        long min = a[0];
        long max = a[0];
        for(int i=0; i<n; i++){
            if(min > a[i]){
                min = a[i];
            }
            if(max < a[i]){
                max = a[i];
            }
        }
        pair p = new pair(min,max);
        return p;
    
    }
}
```
<img width="471" alt="Screenshot 2023-04-15 at 4 04 39 PM" src="https://user-images.githubusercontent.com/111800760/232211381-e248c9d5-e2a5-4b69-ae1d-cfb38e350250.png">

