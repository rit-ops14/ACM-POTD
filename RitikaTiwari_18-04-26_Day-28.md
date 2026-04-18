#Day 28- (subtree of another tree)

##Date - 18/04/26

##Problem - subtree of another tree

##code(C++)- '''class Solution {
public:
    
    bool isSubtree(TreeNode* root, TreeNode* subRoot) {
        if (!root) return false;
        
        if (isSame(root, subRoot)) return true;
        
        return isSubtree(root->left, subRoot) || 
               isSubtree(root->right, subRoot);
    }

    bool isSame(TreeNode* s, TreeNode* t) {
        if (!s && !t) return true;
        if (!s || !t) return false;

        return (s->val == t->val &&
                isSame(s->left, t->left) &&
                isSame(s->right, t->right));
    }
};'''

##Sceenshot-
![Uploading image.png…]()
