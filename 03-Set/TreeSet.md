```java
package jcf_practice;

import java.util.TreeSet;

public class TreeSetDemo {

	public static void main(String[] args) {

		TreeSet<Integer> ts = new TreeSet<>();

		// add()
		ts.add(100);
		ts.add(50);
		ts.add(150);
		ts.add(175);
		ts.add(25);
		ts.add(75);
		ts.add(225);
		ts.add(125);
		ts.add(200);
		
		// TreeSet always stores elements in sorted (ascending) order.
		System.out.println("AFTER add(): " + ts);

		// duplicate element (ignored)
		ts.add(25);
		System.out.println("AFTER ADDING DUPLICATE 25: " + ts);

		// null elements are not allowed in TreeSet

		
		// remove
		ts.remove(150);
		System.out.println("AFTER REMOVING 150: " + ts);

		// size()
		System.out.println("SIZE OF TREESET: " + ts.size());

		// contains()
		System.out.println("CONTAINS 100: " + ts.contains(100));

		// isEmpty()
		System.out.println("IS TREESET EMPTY: " + ts.isEmpty());

		// first()
		System.out.println("FIRST ELEMENT: " + ts.first());

		// last()
		System.out.println("LAST ELEMENT: " + ts.last());

		// clear()
		ts.clear();
		System.out.println("AFTER clear(): " + ts);
	}

}
```
## Iteration styles
1. Enhanced for-each loop
2. Iterator
####  1. Enhanced for-each loop
```java
package jcf_practice;

import java.util.TreeSet;

public class TreeSetDemo {

	public static void main(String[] args) {

		TreeSet<Integer> ts = new TreeSet<>();

		// add()
		ts.add(100);
		ts.add(50);
		ts.add(150);
		ts.add(175);
		ts.add(25);
		ts.add(75);
		ts.add(225);
		ts.add(125);
		ts.add(200);
		
		for(Integer num : ts) {
			System.out.print(num + " ");
		}
	}
}
```