# Algorithms 101 - How to Research Algorithms

## Three useful tools for researching Algorithm

### Content

1. How to print an array to console

2. How to measure the runtime of an algorithm

3. How to write data to file

### How to print an array to console

If you were to run the following code into Eclipse:

```java
public class myClass {
	static int[] myObj = {1, 3984, 394, 394, 49, 763};
	public static void main(String[] args) {
		myMethod(myObj);
	}
	private static void myMethod(int[] myObj) {
		System.out.println(myObj);
	}
}
```

You will get the following output or something similar:

```
[I@d716361
```

This is because an array is a linear data structure which means it's not intended for printing out. So how do we print an array?

To print an array, we need to do the following.

1. First and foremost, we need to get each element of the array in order. To do this we will use a For Loop.

```Java
for (int index = 0; i < n; ++i) {

}
```

2. Once we have an element from the array we can print it. You cannot print an array, but you an print the element inside an array. To do this we will use System.out.print.

```Java
System.out.print(); // Prints Object to current line
System.out.println(); // Prints Object to new line.
```

#### The Result

```java
public class myClass {
	static int[] myObj = {1, 3984, 394, 394, 49, 763};
	public static void main(String[] args) {
		myMethod(myObj);
	}
	private static void myMethod(int[] myObj) {
		int n = myObj.length;
		for (int i = 0; i < n; ++i) {
			System.out.print(myObj[i] + ", ");
		}
	}
}

```
1, 3984, 394, 394, 49, 763, 
```
