# 标题1



## 二级标题

[1. 两数之和](https://leetcode-cn.com/problems/two-sum/)

![](https://pic.leetcode-cn.com/2519bd7f7da0f3bd51dd0f06e6363f4f62bfb25472c5ec233cf969e5c1472e33-file_1559748028103)




```java
class Solution {
    public ListNode reverseList(ListNode head) {
        ListNode prev = null;
        ListNode curr = head;
        while (curr != null) {
            ListNode next = curr.next;
            curr.next = prev;
            prev = curr;
            curr = next;
        }
        return prev;
    }
}
```
//测试代码