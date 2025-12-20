```java
package jcf_practice;

import java.util.ArrayList;
public class ArrayListDemo {

	public static void main(String[] args) {
		ArrayList<Integer> list = new ArrayList<>();

		// add()
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(125);
		list.add(175);
		System.out.println("AFTER add(): " + list);
		
		// add(index, element)
		list.add(0, 200);
		System.out.println("AFTER add(index, element): " + list);
		
		// get()
		System.out.println("get(1): " + list.get(1));
		
		// set()
		list.set(3, 225);
		System.out.println("AFTER set(): " + list);
		
		// remove()
		list.remove(3);
		System.out.println("AFTER remove(): " + list);
		
		// size()
		System.out.println("SIZE OF LIST: " + list.size());
		
		// contains()
		System.out.println("CONTAINS 207: " + list.contains(207));
		
		// indexOf()
		System.out.println("INDEX OF 25: "+ list.indexOf(25));
		
		// isEmpty
		System.out.println("IS LIST EMPTY " + list.isEmpty());
		
		// lastIndexOf()
		list.add(25);
		System.out.println("AFTER add(): " + list);
		System.out.println("LAST INDEX OF 25: " + list.lastIndexOf(25));
		
		// replaceAll()
		list.replaceAll(num -> num == 25 ? 20 : num);
		System.out.println("LIST AFTER REPLACING 25 WITH 20: " + list);
		
		// subList()
		// extracting elements from index 1 (inclusive) to 4 (exclusive)
		 ArrayList<Integer> sub = new ArrayList<>(list.subList(1,  4));
		 System.out.println("SUB LIST (1 TO 4): " + sub);
		 
		// clear()
		 // list.clear();
		 // System.out.println("After clear(): " + list);		
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

import java.util.ArrayList;
public class ArrayListDemo {

	public static void main(String[] args) {
		ArrayList<Integer> list = new ArrayList<>();

		// add()
		list.add(250);
		list.add(100);
		list.add(50);
		list.add(150);
		list.add(25);
		list.add(75);
		list.add(250);
		list.add(125);
		list.add(175);
		list.add(225);

		// classical for loop
		for(int i=0; i<list.size(); i++) {
			System.out.print(list.get(i) + " ");
		}	
	}
}
```
####  2. Enhanced for-each loop
