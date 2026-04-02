#Day 12 - (remove duplicates from sorted lists)

##Date - 02/04/26

##Problem - remove duplicates from sorted list

##code(C++)- '''class Solution {
public:
    ListNode* deleteDuplicates(ListNode* head) {
        if (!head) return nullptr;
        ListNode* current = head;
        while (current && current->next) {
            if (current->val == current->next->val) {
                current->next = current->next->next;
            } else {
                current = current->next;
            }
        }
        return head;
        
    
    }
};'''
##Screenshot-
<img width="1910" height="852" alt="image" src="https://github.com/user-attachments/assets/54dc77d3-80d0-4d4f-b6be-5c4f543c3249" />

