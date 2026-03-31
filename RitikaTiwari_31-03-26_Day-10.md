#Day 10 - (middle of the linked list)

##Date - 31/03/26

##Problem - middle of the linked list

##code(C++)- '''class Solution {
public:
    ListNode* middleNode(ListNode* head) {
        ListNode* slow= head;
        ListNode* fast= head;
        while(fast !=NULL && fast->next !=NULL){
            slow=slow->next;
            fast=fast->next->next;
        }
        return slow;
        
    }
};'''

##Screenshot-
<img width="1515" height="784" alt="image" src="https://github.com/user-attachments/assets/adcc0ded-a663-463e-8d9b-021c39de239d" />
