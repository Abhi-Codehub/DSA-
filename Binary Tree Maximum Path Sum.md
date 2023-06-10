#Maximum Path Sum in Binary tree
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
    public int maxPathSum(TreeNode root) {
            int maxValue[] = new int[1];
            maxValue[0] = Integer.MIN_VALUE;
            maxDownPath (root, maxValue);
            return maxValue[0];
    }
        public int maxDownPath (TreeNode root , int maxValue[]) {
            if(root == null){
                return 0;
            }
            int leftSum = Math.max(0, maxDownPath(root.left, maxValue));
            int rightSum = Math.max(0, maxDownPath(root.right, maxValue));
            maxValue[0] = Math.max(maxValue[0], leftSum + rightSum + root.val);

            return Math.max(leftSum, rightSum) + root.val;

        }
    }
```
<img width="867" alt="Screenshot 2023-06-10 at 5 15 29 PM" src="https://github.com/Abhi-Codehub/DSA-/assets/111800760/1462c1d3-9722-4b1a-9b19-aef01c6c7ce9">
