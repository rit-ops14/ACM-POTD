#Day 23- (find the two judge)

##Date - 13/04/26

##Problem - find the two judge

##code(C++)- '''class Solution {
public:
    int findJudge(int n, vector<vector<int>>& trust) {
        vector<int> in(n+1,0),out(n+1,0);
    for(auto&t:trust){out[t[0]]++;in[t[1]]++;}
    for(int i=1;i<=n;i++)if(in[i]==n-1&&out[i]==0)return i;
    return -1;
    }
};'''

##Screenshot-
<img width="1641" height="837" alt="image" src="https://github.com/user-attachments/assets/a81e7038-4ee8-4c91-8ddb-fd10d9fb2097" />
