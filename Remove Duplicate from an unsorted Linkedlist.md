# Remove Duplicate From an unsorted Linkedlist
```
class Solution
{
    //Function to remove duplicates from unsorted linked list.
    public Node removeDuplicates(Node head) 
    {
         // Your code here
         
         HashSet<Integer> hash = new HashSet<>();
         
         Node curr = head;
         Node prev = null;
         
         while(curr != null){
             int curr_value = curr.data;
             
        if(hash.contains(curr_value)){
            prev.next = curr.next;
        }
        else{
            hash.add(curr_value);
            prev = curr;
            
        }
        curr = curr.next;
        }
         return head;
    }
}
```
<img width="445" alt="Screenshot 2023-08-24 at 9 11 51 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/3947dede-cc82-4c16-8a02-efa862804fc8">

