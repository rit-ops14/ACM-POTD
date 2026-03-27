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
##code(C++)- cpp   OPTIMAL SOLUTION
'''class Solution {
public:
    bool checkIfExist(vector<int>& arr) {
        unordered_set<int>s;
        for(int num:arr){
            if(s.count(2*num)||(num%2==0&&s.count(num/2))){
                return true;
            }
            s.insert(num);
        }      
        return false;
    }
    
};'''

##Screenshot-
<img width="1504" height="786" alt="image" src="https://github.com/user-attachments/assets/ffa3f980-1a88-4875-b90c-8638de14fbb9" />
##OPTIMAL SOLUTION-
<img width="696" height="786" alt="image" src="https://github.com/user-attachments/assets/7cfcec23-9d56-4c72-966d-3948f6f1541b" />
