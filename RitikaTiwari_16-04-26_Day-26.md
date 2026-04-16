#Day 26- (invert binary tree)

##Date - 16/04/26

##Problem - invert binary tree

##code(C++)- '''class Solution {
public:
    TreeNode* invertTree(TreeNode* root) {
        if (!root) return nullptr;
        swap(root->left, root->right);
        invertTree(root->left); invertTree(root->right);
        return root;
        
    }
};'''

##Screenshot-
<img width="1919" height="860" alt="image" src="https://github.com/user-attachments/assets/90f92678-1548-4f13-a796-beb4fa0de9c6" />
