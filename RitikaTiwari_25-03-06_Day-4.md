#Day 4 - (missing number)

##Date - 25/03/26

##Problem - missing number

##Approach - 
i calculated expected sum of n natural numbers for entire range and by traversing the entire array calculated its total actual sum and found the difference that gives me the one missing number

##code(C++)-
'''class Solution {
public:
    int missingNumber(vector<int>& nums) {
        int n= nums.size();
        int expected= n*(n+1)/2;
        int actual= 0;
        for(int x:nums) actual+=x;
        return expected-actual;
        
    }
};'''

##Screenshot-
<img width="526" height="789" alt="image" src="https://github.com/user-attachments/assets/abd5685c-4355-4add-97a1-74aa4c4dc24a" />
