#Day 33- ( min cost climbing stairs )

##Date - 23/04/26

##Problem -min cost climbing stairs

##code(C++)- '''class Solution {
public:
    int minCostClimbingStairs(vector<int>& cost) {
        int n = cost.size();
        int prev1 = cost[0], prev2 = cost[1];
        for (int i = 2; i < n; i++) {
            int current = cost[i] + min(prev1, prev2);
            prev1 = prev2;
            prev2 = current;
        }
        return min(prev1, prev2);
    }
};'''

##Screenshot-
<img width="1527" height="865" alt="image" src="https://github.com/user-attachments/assets/3f34f779-d069-4617-a76c-b91088ba90d3" />
