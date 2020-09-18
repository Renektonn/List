# List
import java.util.*;
public class Main {
	public static void main(String[] args) {
		Scanner cin = new Scanner(System.in);
		int [] arr = {0 , 2 , 6 , 7 , 5 , 3 , 4 , 1};
		Node head = new Node ();
		Node tail = new Node ();
		head.data=arr[0];
		tail=head;
		for(int i = 1;i <= 7;i++ ) {
			Node tem = new Node ();
			tem.data = arr[i];
			tail.next=tem;
			tail=tail.next;

		}
		Node tem = new Node ();
		tem=head;
		for(int i=0;i <= 7; i++) {
			System.out.print(tem.data+" ");
			tem=tem.next;
		}
	}
}
class Node{
	int data;
	Node next;
}
