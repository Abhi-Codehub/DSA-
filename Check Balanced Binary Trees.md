# Check wheether the Binary trees is balanced or not?
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
    public boolean isBalanced(TreeNode root) {
        return dfsHeight(root) != -1;
    }        
    public static int dfsHeight(TreeNode root){
        // base condition 
        if (root == null){
            return 0;
        }
        int leftHeight = dfsHeight(root.left);
        if(leftHeight == -1){
            return -1;
        }
        int rightHeight = dfsHeight(root.right);
        if(rightHeight == -1){
            return -1;
        }
        if (Math.abs(leftHeight - rightHeight) > 1 ){
            return -1;
        }   
         return (Math.max(leftHeight, rightHeight)+1);
    }         
}
```
<img width="868" alt="Screenshot 2023-06-10 at 1 52 12 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/829478a4-2366-43c2-bf89-72438218a305">
