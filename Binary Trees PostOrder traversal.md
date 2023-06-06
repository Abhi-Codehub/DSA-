# Binary Tress postorder traversal
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
        traversal(root.right, res);
        res.add(root.val);
    }

    public List<Integer> postorderTraversal(TreeNode root) {
        List<Integer> res = new ArrayList<>();
        traversal(root, res);
        return res;
        
    }
}
```
<img width="862" alt="Screenshot 2023-06-06 at 9 56 16 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/0ededfc4-c716-4d76-b184-da3aaa2c71f1">
