public static Node reverseDLL(Node  head)
{
    //Your code here
     Node current = head, next = null, previous = null;
    
    while(current != null){
        next = current.next;
        current.prev = next;
        current.next = previous;
        
        previous = current;
        current = next;
    }
return previous;
}
