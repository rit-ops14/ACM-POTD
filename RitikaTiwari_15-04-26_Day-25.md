#Day 25- (maximum depth of binary tree)

##Date - 15/04/26

##Problem - maximum depth of binary tree


##code(C++)- '''class Solution {
public:
    int maxDepth(TreeNode* root) {
        if (!root) return 0;
        return 1 + max(maxDepth(root->left), maxDepth(root->right));
    }
};'''

##Screenshot-
<img width="1772" height="803" alt="image" src="https://github.com/user-attachments/assets/76af11c3-e49b-4581-8b6d-3b6ba4726b3d" />
