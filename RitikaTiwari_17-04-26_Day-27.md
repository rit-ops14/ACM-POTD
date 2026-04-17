#Day 27- (diameter of binary tree)

##Date - 17/04/26

##Problem - diameter of binary tree

##code(C++)- '''class Solution {
public:
    int diameterOfBinaryTree(TreeNode* root) {
        int ans=0;
        function<int(TreeNode*)> h=[&](TreeNode* node)->int{
            if(!node)return 0;
            int l=h(node->left),r=h(node->right);
            ans=max(ans,l+r); return 1+max(l,r);
        };
        h(root); return ans;
    }
};'''
##Screenshot-
<img width="1880" height="857" alt="image" src="https://github.com/user-attachments/assets/61924de3-11aa-4aa1-9ebb-7652e81eb723" />
