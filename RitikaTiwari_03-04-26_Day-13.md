#Day 13- (intersection of two linked lists)

##Date - 03/04/26

##Problem - intersection of two linked lists)


##code(C++)- '''class Solution {
public:
    ListNode *getIntersectionNode(ListNode *headA, ListNode *headB) {
        if (!headA || !headB) return nullptr;
        ListNode *pA = headA, *pB = headB;
        
        while (pA != pB) {
            pA = !pA ? headB : pA->next;
            pB = !pB ? headA : pB->next;
        }
        return pA;
        
    }
};'''
