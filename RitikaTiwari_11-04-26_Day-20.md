#Day 20- (make string great)

##Date - 11/04/26

##Problem - make string great


##code(C++)- '''class Solution {
public:
    string makeGood(string s) {
        string st;
    for (char c : s) {
        if (!st.empty()&&abs(st.back()-c)==32) st.pop_back();
        else st+=c;
    }
    return st;
        
    }
};'''
