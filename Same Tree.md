#Check whether the trees are same or not ?
```
/**
 * Definition for a binary tree node.
 * public class TreeNode {
 *     int val;
 *     TreeNode left;
 *     TreeNode right;
 *     TreeNode() {}
 *     TreeNode(int val) { this.val = val; }
 *     TreeNode(int val, TreeNode left, TreeNode right) {
 *         this.val = val;
 *         this.left = left;
 *         this.right = right;
 *     }
 * }
 */
class Solution {
    public boolean isSameTree(TreeNode p, TreeNode q) {
        if(p == null || q == null){
             return (p == q);
        }
       return (p.val == q.val) && isSameTree(p.left, q.left) && isSameTree(p.right, q.right);
    }
}
```
<img width="827" alt="Screenshot 2023-06-11 at 12 10 03 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/02a21f83-aebe-4a58-87a5-23ea590e5f71">
