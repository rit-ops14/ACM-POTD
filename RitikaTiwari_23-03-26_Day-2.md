#Day 2 - (two sum)

##Date - 23/03/26

##Problem - two sum

##Approach - 
i took nested loop for two pointers and by keeping one pointer i as it is and checking other pointer sum with i to match with target and return its index

##Code (C++)
'''class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
        int n = nums.size();
        for(int i=0;i<n;i++){
            for(int j=i+1;j<n;j++){
                if(nums[i]+nums[j]==target){
                    return{i,j};
                }
               
            }
        }
        return{};
        
    }
};'''
##screenshot-
<img width="769" height="796" alt="image" src="https://github.com/user-attachments/assets/0156959b-3500-459e-8aef-2245cd805753" />

