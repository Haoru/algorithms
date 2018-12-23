Problem Analysis
===========
Remove Duplicates from Sorted List
----------
Given a sorted linked list, delete all duplicates such that each element appear only once.

Programming Implementation
===============
```python
class Solution:
    def deleteDuplicates(self, head):
        """
        :type head: ListNode
        :rtype: ListNode
        """
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
