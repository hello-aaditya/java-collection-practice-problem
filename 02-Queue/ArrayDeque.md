# `ArrayDeque`
```java
package jcf_practice;

import java.util.ArrayDeque;

public class ArrayDequeDemo {

	public static void main(String[] args) {
		ArrayDeque<Integer> dq = new ArrayDeque<>();

		// add() -> adds element at tail
		dq.add(100);
		dq.add(50);
		dq.add(150);
		dq.add(175);
		dq.add(25);
		dq.add(75);
		dq.add(125);
		System.out.println("AFTER add(): " + dq);

		// addFirst()
		dq.addFirst(200);
		System.out.println("AFTER addFirst(): " + dq);

		// addLast()
		dq.addLast(225);
		System.out.println("AFTER addLast(): " + dq);

		// offer() -> adds element at tail
		dq.offer(5);
		System.out.println("AFTER offer(): " + dq);

		// offerFirst()
		dq.offerFirst(0);
		System.out.println("AFTER offerFirst(): " + dq);

		// offerLast()
		dq.offerLast(-25);
		System.out.println("AFTER offerLast(): " + dq);

		// peek() -> look at first element (does not remove)
		System.out.println("peek(): " + dq.peek());

		// peekFirst() -> look at first element (does not remove)
		System.out.println("peek(): " + dq.peekFirst());

		// peekLast() -> look at last element (does not remove)
		System.out.println("peek(): " + dq.peekLast());

		// poll() -> pull the first element (remove)
		System.out.println("poll(): " + dq.poll());
		System.out.println("AFTER poll(): " + dq);

		// pollFirst() -> pull the first element (remove)
		System.out.println("pollFirst(): " + dq.pollFirst());
		System.out.println("AFTER pollFirst(): " + dq);
		
		// pollLast() -> pull the last element (remove)
		System.out.println("pollLast(): " + dq.pollLast());
		System.out.println("AFTER pollLast(): " + dq);
		
		// size()
		System.out.println("SIZE OF DEQUE: " + dq.size());
		
		// contains()
		System.out.println("CONTAINS 150: " + dq.contains(150));
		
		// isEmpty()
		System.out.println("IS DEQUE EMPTY: " + dq.isEmpty());
		
		// clear()
		dq.clear();
		System.out.println("AFTER CLEAR(): " + dq);
	}

}
```