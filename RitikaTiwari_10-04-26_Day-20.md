#Day 20- (remove outer parenthesis)

##Date - 10/04/26

##Problem - remove outer parenthesis


##code(C++)- '''class Solution {
public:
    string removeOuterParentheses(string s) {
        string result = "";
        int balance = 0;
        for (char c : s) {
            if (c == '(') {
                if (balance > 0) result += c;
                balance++;
            } else {
                balance--;
                if (balance > 0) result += c;
            }
        }
        return result;
        
    }
};'''
