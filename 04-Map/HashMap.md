```java
package jcf_practice;

import java.util.HashMap;
public class HashMapDemo {

	public static void main(String[] args) {
		HashMap<Integer, String> map =  new HashMap<>();
		
		// put()
		map.put(51, "Java");
		map.put(52, "DSA");
		map.put(53, "SQL");
		map.put(54, "JavaScript");
		map.put(55, "React.JS");
		// printing order may vary
		System.out.println("AFTER put(): " + map);
		
		// duplicate key (value replaced)
		map.put(55, "DevOps");
		System.out.println("AFTER PUTTING DUPLICATE KEY 55: " + map);
		
		// null key (allowed once)
		map.put(null, "nullKey");
		System.out.println("AFTER ADDING null KEY: " + map);
		
		// null values (allowed multiple times)
		map.put(57,  null);
		map.put(58, null);
		System.out.println("AFTER ADDING null VALUES: " + map);
		
		// get()
		System.out.println("VALUE FOR KEY 52: " + map.get(52));
		
		// remove()
		map.remove(58);
		System.out.println("AFTER remove(58): " + map);
		
		// containsValue()
		System.out.println("CONTAINS VALUE 'Java': " + map.containsValue("Java"));
		
		// containsKey()
		System.out.println("CONTAINS KEY 53: " + map.containsKey(53));
		
		// size()
		System.out.println("CURRENT MAP: " + map);
		System.out.println("SIZE OF MAP: " + map.size());
		
		// isEmpty()
		System.out.println("IS MAP EMPTY: " + map.isEmpty());
		
		// clear()
		map.clear();
		System.out.println("AFTER clear(): " + map);
		
	}

}
```
