/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode() {}
 *     ListNode(int val) { this.val = val; }
 *     ListNode(int val, ListNode next) { this.val = val; this.next = next; }
 * }
 */
// 0 1 2 3 4 5 6
// 1 2 3 4 5 6 7
class Solution {
    public ListNode removeNthFromEnd(ListNode head, int n) {
        
        ListNode temp = head;
        ListNode node = head;
        if(node.next==null)
         return null;
        int flag=0;
        for(int i=1;node.next!=null;i+=n)
        {  
            ListNode last=node;

            for(int j=1;j<=i;j++)
            {
                if(node.next==null)
                { System.out.println("break"); flag=1; break;}
                node=node.next;   
            }
            if(flag==1)
            {
                node=last;
                break;
            }
        }
        // node=node.next;
        System.out.println(node.val);
        node.val=node.next.val;
        node.next=node.next.next;
        
        return temp;
    }
}
