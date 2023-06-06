# Inorder Traversal
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
    public void traversal(TreeNode root, List<Integer> res){
        if(root == null){
            return;
        }
            traversal(root.left, res);
            res.add(root.val);
            traversal(root.right, res);
    }

    public List<Integer> inorderTraversal(TreeNode root) {

        List<Integer> res = new ArrayList<>();
        traversal(root,res);
        return res;
    }
}
```
<img width="1192" alt="Screenshot 2023-06-06 at 9 37 27 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/e0cbee5e-bd15-4d68-94d9-8dbd6fd6263e">
