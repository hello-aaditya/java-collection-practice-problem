# `PriorityQueue`
```java
package jcf_practice;

import java.util.PriorityQueue;

public class PriorityQueueDemo {

	public static void main(String[] args) {
		PriorityQueue<Integer> pq = new PriorityQueue<>();

		// add()
		pq.add(100);
		pq.add(50);
		pq.add(150);
		pq.add(175);
		pq.add(25);
		pq.add(75);
		pq.add(225);
		pq.add(125);
		pq.add(200);
		System.out.println("AFTER add(): " + pq); // ❌ Not sorted view

		// offer() -> preferred for queues
		pq.offer(5);
		System.out.println("AFTER offer(): " + pq);

		// peek() -> look
		System.out.println("peek(): " + pq.peek()); // ✔ Smallest element

		// poll() -> pull first element
		System.out.println("poll(): " + pq.poll());
		System.out.println("AFTER poll(): " + pq);

		// size()
		System.out.println("SIZE OF PRIORITY QUEUE: " + pq.size());

		// contains()
		System.out.println("CONTAINS 75: " + pq.contains(75));

		// isEmpty()
		System.out.println("IS PRIORITY QUEUE EMPTY: " + pq.isEmpty());
		
		// clear()
		pq.clear();
		System.out.println("AFTER clear(): " + pq);
	}
}
```
## Iteration styles
1. Enhanced for-each loop
2. Iterator
####  1. Enhanced for-each loop
```java
package jcf_practice;

import java.util.PriorityQueue;

public class PriorityQueueDemo {

	public static void main(String[] args) {
		PriorityQueue<Integer> pq = new PriorityQueue<>();

		// add()
		pq.add(100);
		pq.add(50);
		pq.add(150);
		pq.add(175);
		pq.add(25);
		pq.add(75);
		pq.add(225);
		pq.add(125);
		pq.add(200);
		
		for(int num : pq) {
			System.out.print(num + " ");
		}
	}
}
```