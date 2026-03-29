#Day 8 - (reverse linked list)

##Date - 29/03/26

##Problem - reverse linked list

##code(C++)- 
'''class Solution {
public:
    ListNode* reverseList(ListNode* head) {
        if(head==NULL||head->next==NULL){
            return head;
        }
        ListNode* prev=NULL;
        ListNode* current=head;
        while(current!=NULL){
            ListNode* next=current->next;
            current->next=prev;
            prev = current;
            current = next;

            
        }        
        return prev;
    }
};'''

##Screenshot-
<img width="1713" height="809" alt="image" src="https://github.com/user-attachments/assets/7de232d8-464e-41c0-91ca-55e1b9141c9f" />
