Problem Analysis
===========
Remove Duplicates from Sorted List
----------
Given a sorted linked list, delete all duplicates such that each element appear only once.

Programming Implementation
===============
```python
class ListNode:
     def __init__(self, x):
         self.val = x
         self.next = None
class Solution:
    def deleteDuplicates(self, head):
        if not head:
            return None
        cur=head
        pre=head.next
        while pre:
            if(cur.val==pre.val):
                pre=pre.next
                cur.next=pre
            else:
                cur=cur.next
                pre=pre.next
        return head
 ```
Summarize
=======
It is significance to use pointer. .next is used to indicate the next value of this node.
