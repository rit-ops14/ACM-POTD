#Day 11 - (merge two sorted lists)

##Date - 01/04/26

##Problem - merge two sorted lists

##code(C++)- 
'''class Solution {
public:
    ListNode* mergeTwoLists(ListNode* list1, ListNode* list2) {
        ListNode* dummy = new ListNode(0);
        ListNode* current = dummy;
        while(list1 && list2){
            if(list1->val <= list2->val){
                current->next=list1;
                list1=list1->next;
            }else{
                current->next=list2;
                list2=list2->next;

            }
            current=current->next;
        }
        current->next=list1?list1:list2;
        return dummy->next;
        
    }
};'''

##Screenshot-
<img width="1605" height="850" alt="image" src="https://github.com/user-attachments/assets/f18c1200-89a7-485e-ba10-6fa4e7d10314" />

