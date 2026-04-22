#Day 32- ( pascal's triangle )

##Date - 22/04/26

##Problem -pascal's triangle

##code(C++)- '''class Solution {
public:
    vector<vector<int>> generate(int numRows) {
        vector<vector<int>> result;
        for (int i = 0; i < numRows; i++) {
            vector<int> row(i + 1, 1);
            for (int j = 1; j < i; j++) {
                row[j] = result[i-1][j-1] + result[i-1][j];
            }
            result.push_back(row);
        }
        return result;
    }
};'''

##Screenshot-
<img width="1569" height="793" alt="image" src="https://github.com/user-attachments/assets/72edec53-e64c-4e68-b5e4-9e6b3f8fd3a7" />
