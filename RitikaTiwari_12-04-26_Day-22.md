#Day 22- (flood fill)

##Date - 12/04/26

##Problem - flood fill


##code(C++)- '''class Solution {
public:
    void dfs(vector<vector<int>>& image, int r, int c, int oldColor, int newColor) {
        int n = image.size();
        int m = image[0].size();

        
        if (r < 0 || c < 0 || r >= n || c >= m || image[r][c] != oldColor)
            return;

        
        image[r][c] = newColor;

       
        dfs(image, r+1, c, oldColor, newColor);
        dfs(image, r-1, c, oldColor, newColor);
        dfs(image, r, c+1, oldColor, newColor);
        dfs(image, r, c-1, oldColor, newColor);
    }

    vector<vector<int>> floodFill(vector<vector<int>>& image, int sr, int sc, int newColor) {
        int oldColor = image[sr][sc];

        if (oldColor == newColor) return image;

        dfs(image, sr, sc, oldColor, newColor);
        return image;
    }
};'''

##Screenshot-
<img width="1578" height="795" alt="image" src="https://github.com/user-attachments/assets/e580d5b9-62d5-44e9-a38c-d2620bc6d63b" />


