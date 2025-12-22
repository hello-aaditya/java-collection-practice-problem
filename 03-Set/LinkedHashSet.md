# `LinkedHashSet`
```java
package jcf_practice;

import java.util.LinkedHashSet;

public class LinkedHashSetDemo {

	public static void main(String[] args) {

		LinkedHashSet<Integer> lhs = new LinkedHashSet<>();

		// add()
		lhs.add(100);
		lhs.add(50);
		lhs.add(150);
		lhs.add(175);
		lhs.add(25);
		lhs.add(75);
		lhs.add(225);
		lhs.add(125);
		lhs.add(200);
		System.out.println("AFTER add(): " + lhs);

		// duplicate element (ignored)
		lhs.add(25);
		System.out.println("AFTER ADDING DUPLICATE 25: " + lhs);

		// add null (allowed once)
		lhs.add(null);
		System.out.println("AFTER ADDING null: " + lhs);
		
		// add null again (ignored)
		lhs.add(null);
		System.out.println("AFTER ADDING null AGAIN: " + lhs);
		
		// remove()
		lhs.remove(225);
		System.out.println("AFTER REMOVING(225): " + lhs);
		
		// size()
		System.out.println("SIZE OF LINKEDHASHSET: " + lhs.size());
		
		// contains()
		System.out.println("CONTAINS 100: " + lhs.contains(100));
		
		// isEmpty()
		System.out.println("IS LINKEDHASHSET EMPTY: " + lhs.isEmpty());
		
		// clear()
		lhs.clear();
		System.out.println("AFTER clear(): " + lhs);
	}

}
```
## Iteration styles
1. Enhanced for-each loop
2. Iterator
