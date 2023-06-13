# Linked List Cycle
```
/**
 * Definition for singly-linked list.
 * class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode(int x) {
 *         val = x;
 *         next = null;
 *     }
 * }
 */
public class Solution {
    public boolean hasCycle(ListNode head) {
        ListNode slow = head, fast = head;
        while(fast!=null && fast.next!=null){
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

<img width="771" alt="Screenshot 2023-06-13 at 8 00 52 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/24da6eb8-048b-4486-8ab2-e471f69cb4af">

