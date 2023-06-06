#Maximum Depth of Binary Tree
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
    public int maxDepth(TreeNode root) {

        if(root == null){
            return 0;
        }
        int leftHeight = maxDepth(root.left);
        int rightHeight = maxDepth(root.right);

        int myHeight = Math.max(leftHeight, rightHeight) + 1;
        
        return myHeight;
    }
}
```
<img width="853" alt="Screenshot 2023-06-07 at 12 15 58 AM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/5a2eea5d-5fab-4c0e-ac8f-bb87f8cc4591">
