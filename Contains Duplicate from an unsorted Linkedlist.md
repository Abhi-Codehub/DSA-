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
