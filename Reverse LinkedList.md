# Reverse LinkedList 
```
/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
class Solution {

    public ListNode reverseList(ListNode head) {
         if(head == null){
            return head;
        }
        ListNode curr = head;
        ListNode prev = null;
    
    while(curr!= null){
        ListNode temp = curr.next;
        curr.next = prev;
        prev = curr;
        curr = temp;
        
    }
    return prev;
    }
        
}
```
<img width="788" alt="Screenshot 2023-06-13 at 8 45 55 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/4358d974-b96a-4ebe-bd7e-4f031f9fc993">


