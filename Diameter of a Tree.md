# Diameter of a Tree
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

    public static int height(TreeNode root){
        if(root == null){
            return 0;
        }
        int leftHeight = height(root.left);
        int rightHeight = height(root.right);

        int maxHeight = Math.max(leftHeight, rightHeight) + 1;
        return maxHeight;
    }
    public int diameterOfBinaryTree(TreeNode root) {

        if(root == null){
            return 0;
        }
        int diam1 = diameterOfBinaryTree(root.left);
        int diam2 = diameterOfBinaryTree(root.right);
        int diam3 = height(root.left) + height(root.right) ;
        
        return Math.max(diam3, Math.max(diam1,diam2));
    }
}
```
<img width="863" alt="Screenshot 2023-06-07 at 11 27 30 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/a124cde0-e142-4ee3-81c0-50fc040f048f">

