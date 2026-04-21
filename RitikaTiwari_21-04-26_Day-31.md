#Day 31- ( climbing stairs )

##Date - 21/04/26

##Problem -climbing stairs  

##code(C++)- '''class Solution {
public:
    int climbStairs(int n) {
        if (n <= 2) return n;
        int prev = 1, curr = 2;
        for (int i = 3; i <= n; i++) {
            int temp = prev + curr;
            prev = curr;
            curr = temp;
        }
        return curr;
    
    }
};'''

##Screenshot-
<img width="1745" height="805" alt="image" src="https://github.com/user-attachments/assets/274ea288-436a-4535-a366-707de6855d8b" />
