#Day 19- (backspace string compare)

##Date - 09/04/26

##Problem - backspace string compare


##code(C++)- '''class Solution {
public:
    bool backspaceCompare(string s, string t) {
        int i = s.size() - 1;
        int j = t.size() - 1;

        int skipS = 0, skipT = 0;

        while (i >= 0 || j >= 0) {
            while (i >= 0) {
                if (s[i] == '#') {
                    skipS++;
                    i--;
                } else if (skipS > 0) {
                    skipS--;
                    i--;
                } else break;
            }

            while (j >= 0) {
                if (t[j] == '#') {
                    skipT++;
                    j--;
                } else if (skipT > 0) {
                    skipT--;
                    j--;
                } else break;
            }

            if (i >= 0 && j >= 0) {
                if (s[i] != t[j]) return false;
            } else {
                if (i >= 0 || j >= 0) return false;
            }

            i--; j--;
        }
        return true;
        
    }
};'''

##Screenshot- <img width="1796" height="857" alt="image" src="https://github.com/user-attachments/assets/c7a1ead9-fc84-44c8-8495-2bffedaf342c" />
