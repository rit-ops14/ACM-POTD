#Day 7 - (rotate array)

##Date - 28/03/26

##Problem - rotate array

##code(C++)-
'''class Solution {
public:
    void rotate(vector<int>& nums, int k) {
        int n= nums.size();
        vector<int> temp(n);
        for(int i=0;i<n;i++){
            temp[(i+k)%n]=nums[i];
           
        }
        nums=temp;
        
    }
};'''

##Screenshot-
<img width="591" height="803" alt="image" src="https://github.com/user-attachments/assets/72dc6d73-ac41-4c2e-b184-bf8e65aa3d20" />
