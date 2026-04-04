#Day 14- (palindrome lists)

##Date - 04/04/26

##Problem - palindrome lists


##code(C++)- '''class Solution {
public:
    bool isPalindrome(ListNode* head){
        if (!head || !head->next) return true;
        
        ListNode* slow = head, *fast = head;
        while (fast && fast->next) {
            slow = slow->next;
            fast = fast->next->next;
        }
        
        ListNode* prev = nullptr;
        while (slow) {
            ListNode* next = slow->next;
            slow->next = prev;
            prev = slow;
            slow = next;
        }
        
        ListNode* left = head, *right = prev;
        while (right) {
            if (left->val != right->val) return false;
            left = left->next;
            right = right->next;
        }
        return true;
        
    }
};'''
