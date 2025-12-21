# `HashSet`
```java
package jcf_practice;

import java.util.HashSet;

public class HashSetDemo {

	public static void main(String[] args) {

		HashSet<Integer> hs = new HashSet<>();

		// add()
		hs.add(100);
		hs.add(50);
		hs.add(150);
		hs.add(175);
		hs.add(25);
		hs.add(75);
		hs.add(225);
		hs.add(125);
		hs.add(200);
		System.out.println("AFTER add(): " + hs);

		// duplicate element (ignored)
		hs.add(75);
		System.out.println("AFTER ADDING DUPLICATE 75: " + hs);

		// add null (allowed once)
		hs.add(null);
		System.out.println("AFTER ADDING null: " + hs);

		// add null again (ignored)
		hs.add(null);
		System.out.println("AFTER ADDING null AGAIN: " + hs);

		// remove() -> removes specified element
		hs.remove(200);
		System.out.println("AFTER REMOVING(200): " + hs);

		// size()
		System.out.println("SIZE OF SET: " + hs.size());

		// contains()
		System.out.println("CONTAINS 100: " + hs.contains(100));

		// isEmpty()
		System.out.println("IS SET EMPTY: " + hs.isEmpty());

		// clear()
		hs.clear();
		System.out.println("AFTER clear(): " + hs);
	}

}
```
