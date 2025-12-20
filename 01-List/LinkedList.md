# `LinkedList`
```java
package jcf_practice;

import java.util.LinkedList;
public class LinkedListDemo {

	public static void main(String[] args) {
		LinkedList<Integer> list = new LinkedList<>();

		// add()
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(200);
		list.add(250);
		list.add(125);
		list.add(175);
		list.add(25);
		list.add(225);
		System.out.println("AFTER add(): " + list);
		
		// addFirst()
		list.addFirst(999);
		System.out.println("AFTER addFirst(): " + list);
		
		// addLast()
		list.addLast(999);
		System.out.println("AFTER addLast(): " + list);
		
		// get()
		System.out.println("get(2): " + list.get(2));
		
		// getFirst()
		System.out.println("getFirst(): " + list.getFirst());
		
		// getLast()
		System.out.println("getLast(): " + list.getLast());
		
		// set()
		list.set(4,  275);
		System.out.println("AFTER set(): " + list);
		
		// remove() -> removes first element (acts like removeFirst())
		list.remove(); // remove first element
		System.out.println("AFTER remove(): " + list);
		
		list.remove(9); // remove element at mentioned index
		System.out.println("AFTER remove(9): " + list);
		
		// removeLast()
		list.removeLast();
		System.out.println("AFTER removeLast(): " + list);
		
		// size()
		System.out.println("SIZE OF LIST: " + list.size());
		
		// contains()
		System.out.println("CONTAINS 75: " + list.contains(75));
		
		// add()
		list.add(1, 25);
		list.add(8, 25);
		System.out.println("AFTER add(): " + list);
		
		// indexOf()
		System.out.println("INDEX OF 25: " + list.indexOf(25));
		
		// lastIndexOf()
		System.out.println("LAST INDEX OF 25: " + list.lastIndexOf(25));
		
		// isEmpty()
		System.out.println("IS LIST EMPTY: " + list.isEmpty());
		
		// clear()
		// list.clear();
		// System.out.println("AFTER clear(): " + list);
	}
}
```

## Iteration styles
1. Classical for-loop
2. Enhanced for-each loop
3. Iterator
#### 1. Classical for-loop
```java
package jcf_practice;

import java.util.LinkedList;
public class LinkedListDemo {

	public static void main(String[] args) {
		LinkedList<Integer> list = new LinkedList<>();

		// add()
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(200);
		list.add(250);
		list.add(125);
		list.add(175);
		list.add(25);
		list.add(225);
		
		// classical for-loop
		for(int i=0; i<list.size(); i++) {
			System.out.print(list.get(i) + " ");
		}
	}
}
```
####  2. Enhanced for-each loop
```java
package jcf_practice;

import java.util.LinkedList;
public class LinkedListDemo {

	public static void main(String[] args) {
		LinkedList<Integer> list = new LinkedList<>();

		// add()
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(200);
		list.add(250);
		list.add(125);
		list.add(175);
		list.add(25);
		list.add(225);
		
		// enhanced for-loop
		for(int num : list) {
			System.out.print(num + " ");
		}
	}
}
```
#### 3. Iterator
```java
package jcf_practice;

import java.util.LinkedList;
import java.util.Iterator;
public class LinkedListDemo {

	public static void main(String[] args) {
		LinkedList<Integer> list = new LinkedList<>();

		// add()
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(200);
		list.add(250);
		list.add(125);
		list.add(175);
		list.add(25);
		list.add(225);
		
		// iterator
		Iterator<Integer> itr = list.iterator();
		
		while(itr.hasNext()) {
			System.out.print(itr.next() + " ");
		}
	}
}
```
