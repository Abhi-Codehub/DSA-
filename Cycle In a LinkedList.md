# Detect cycle in a Linkedlist 
```
class Solution {
    //Function to check if the linked list has a loop.
    public static boolean detectLoop(Node head){
        // Add code here
        Node slow = head;
        Node fast = head;
        
        while(fast != null && fast.next != null){
        slow = slow.next;
        fast = fast.next.next;
        if(slow == fast){
            return true;
        }
        
        } 
        return false;
    }
}
```
<img width="434" alt="Screenshot 2023-08-23 at 3 39 26 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/d8458ee8-9c42-4e64-b92d-7f671d310177">

