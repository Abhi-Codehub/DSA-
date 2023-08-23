# Merge two sorted list
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
    public ListNode mergeTwoLists(ListNode list1, ListNode list2) {

        ListNode tempList = new ListNode(0);
        ListNode current_node = tempList;

        while(list1 != null && list2 != null){

        if(list1.val < list2.val){
            current_node.next = list1;
            list1 = list1.next;
        }
        else {
            current_node.next = list2;
            list2 = list2.next;
        }
        current_node = current_node.next;
      }
      if(list1 != null){
          current_node.next = list1;
          list1 = list1.next;
      }
      if(list2 != null){
          current_node.next = list2;
          list2 = list2.next;
      }
      return tempList.next;
    }
}
```
<img width="744" alt="Screenshot 2023-08-23 at 6 29 05 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/8f674494-b7b9-4ed8-8992-fb768e0791eb">

