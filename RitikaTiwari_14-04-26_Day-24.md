#Day 24- (find center of star graph)

##Date - 04/04/26

##Problem - find the center of star graph


##code(C++)- '''class Solution {
public:
    int findCenter(vector<vector<int>>& edges) {
        return (edges[0][0]==edges[1][0]||edges[0][0]==edges[1][1])?edges[0][0]:edges[0][1];
        
    }
}'''

##Screenshot-
<img width="1575" height="823" alt="image" src="https://github.com/user-attachments/assets/b0ad54a1-6c26-4936-bee6-25bf75c6f51c" />
