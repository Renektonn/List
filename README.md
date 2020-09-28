
import java.util.*;
public class Main {
	public static void main(String[] args) {
		Scanner cin = new Scanner(System.in);
		int [] arr = {0 , 2 , 6 , 7 , 5 , 3 , 4 , 1};
		//init
		Node head = new Node ();
		Node tail = new Node ();
		head.data=arr[0];
		tail=head;
		//add
		for(int i = 1;i <= 7;i++ ) {
			addNode(arr[i],tail);
			tail=tail.next;
		}
		//output
		Node tem = new Node ();
		tem=head;
		for(int i=0;i <= 7; i++) {
			System.out.print(tem.data+" ");
			tem=tem.next;
		}
	}
	static void addNode(int data,Node node) {
		Node tem = new Node ();
		tem.data = data;
		node.next=tem;
		
	}
}
class Node{
	int data;
	Node next;
}
