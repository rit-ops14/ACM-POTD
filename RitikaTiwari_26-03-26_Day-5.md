#Day 5 - (move zeroes)

##Date - 26/03/26

##Problem - move zeroes

##Approach - I maintain a pointer i for the next position of a non-zero. As I iterate with j, whenever I find a non-zero element, I swap it with index i and increment i.
             ensuring O(n) time complexity and no extra spaces i.e., O(1) space complexity.

##code(C++)-
'''class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int n= nums.size();
        int i=0;
        for (int j=0;j<n;j++){
            if(nums[j]!=0){
                swap(nums[i],nums[j]);
                i++;
            }
        }
        

        
    }
};'''

##Screenshot-
<img width="1814" height="784" alt="image" src="https://github.com/user-attachments/assets/ebbad3a9-c077-4d59-bafc-70322e700aa1" />
