#Day 3 - (buy and sell stocks)

##Date - 24/03/26

##Problem - buy and sell stocks

##Approach - 
i took 0th index price and stored it as minimum value for reference then after initializing profit i compared the difference of each incremented pointer i.e., prices with mini value to check for maximum profit and increment it accordingly

##Code (C++)
'''class Solution {
public:
    int maxProfit(vector<int>& prices) {
        int mini= prices[0];
        int maxProfit=0;
        for(int i=0;i<prices.size();i++){
            int cost= prices[i]-mini;
            maxProfit=max(maxProfit,cost);
            mini=min(mini,prices[i]);
        }
        return maxProfit;

        
    }
};'''

##screenshot-
<img width="592" height="745" alt="image" src="https://github.com/user-attachments/assets/066e23ac-3303-481f-bad1-aba8e2c8fa8f" />

