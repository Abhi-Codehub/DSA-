# Reverse LinkedList using iteration 
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

# Reverse Linked List using Recursion 
```
class Solution {

    public ListNode reverse (ListNode head){
        if (head.next == null){
            return head;
        }
        ListNode reverseHead = reverse(head.next);
            head.next.next = head;
            head.next = null;
            return reverseHead;
    }

    public ListNode reverseList(ListNode head) {
        if(head == null){
            return null;
        }
        return reverse(head);
    }
}
```
<img width="724" alt="Screenshot 2023-08-10 at 12 27 31 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/a9626b2f-44b1-484b-b64e-604285ac3d62">



