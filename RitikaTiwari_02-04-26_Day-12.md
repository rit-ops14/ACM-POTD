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
