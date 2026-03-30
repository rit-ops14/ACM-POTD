#Day 9 - (linked list cycle)

##Date - 30/03/26

##Problem - linked list cycle

##code(C++)- '''class Solution {
public:
    bool hasCycle(ListNode *head) {
        if(head==NULL||head->next==NULL) return false;
        ListNode* slow=head;
        ListNode* fast=head;
        while(fast!=NULL && fast->next!=NULL){
            slow=slow->next;
            fast=fast->next->next;
            if(slow==fast) return true;        
        }
        return false;


        
    }
};'''

##Screenshot-
<img width="1717" height="807" alt="image" src="https://github.com/user-attachments/assets/748dad89-1efb-4789-808d-569c5f014f25" />
