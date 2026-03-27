#Day 6 - (check if n and its double exists)

##Date - 27/03/26

##Problem - check if n and its double exists

##Approach - I  have used my brute force logic where i've taken two pointers and by taking nested loops i checked if both the pointers not match with same index and element at ith index is double the element at jth index then return true 

##code(C++)-
'''class Solution {
public:
    bool checkIfExist(vector<int>& arr) {
        int n= arr.size();
        
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
                if(i!=j && arr[i]==2*arr[j]){
                    return true;
                }
            }
        }
        return false;
            
       
        
    }
    
};'''

##Screenshot-
<img width="1504" height="786" alt="image" src="https://github.com/user-attachments/assets/ffa3f980-1a88-4875-b90c-8638de14fbb9" />
