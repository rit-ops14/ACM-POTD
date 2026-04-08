#Day 18- (removing duplicates from string)

##Date - 08/04/26

##Problem - removing duplicates from string


##code(C++)- '''class Solution {
public:
    string removeDuplicates(string s) {
        string st = "";
        for (char c : s) {
            if (!st.empty() && st.back() == c) {
                st.pop_back();
            } else {
                st.push_back(c);
            }
        }
        return st;
        
    }
};'''
