# Day1:

## Wrapper Class
1. Wrapper Class: A Wrapper class is a class whose object wraps or contains primitive data types. When we create an object to a wrapper class, it contains a field and in this field, we can store primitive data types. In other words, we can wrap a primitive value into a wrapper class object.
2. AutoBoxing: Automatic conversion of primitive types to the object of their corresponding wrapper classes is known as autoboxing.
3. UnBoxing:  It is just the reverse process of autoboxing. Automatically converting an object of a wrapper class to its corresponding primitive type is known as unboxing.

## ArrayList in Java
ArrayList is dynamic in nature it can increase and decrease its size.

1. Initialization of ArrayList.
```
ArrayList<String> fruits = new ArrayList<>();
```
Here we cany use any wrapper class instead of String.
2. Adding elements in ArrayList using add() method.
```
fruits.add("Apple");
fruits.add("Banana");
fruits.add("Grapes");
```
3. Adding elements at specific index using overloaded add() method.
```
fruits.add(0, "AddAt0");
fruits.add(2, "AddAt2");
```
This is an overloaded method in which we will specify the index and the value to be added.
4. Accessing elements in ArrayList using get() method.
```
System.out.println(fruits.get(0));
System.out.println(fruits.get(3));
```
5. Updating elements in ArrayList using set() method by appling specific index.
```
fruits.set(0, "update1");
fruits.set(4, "update3");
```
Since String are immutabe in java so it will not change the string instead Object reference is changed to new changed object and the Garbage collector of java will auto remove the old value which is not referencing to any reference.
6. Removing elements in ArrayList using remove() element by index.
```
fruits.remove(1);
fruits.remove(3);
```
removing elements in ArrayList using remove() by value.
```
fruits.remove("update1");
```
removing all elements using clear() method.
```
fruits.clear();
```
7. To find the size of ArrayList using size() method.
```
System.out.println(fruits.size());
```

## 2-D Array

1. Declaring of 2-D Array
```
int[][] numbers = new int[5][3];
```
2. Accessing elements and initalizing it.
```
numbers[0][0] = 3;
numbers[0][1] = 4;
numbers[1][0] = 5;
numbers[1][1] = 6;
```
3. Initialization of 2-D array in a single line.
```
int[][] num = {{1,2,},{4,5}};
```
4. Printing Arrays row by row.
```
for(int i=0;i<2;i++) {
  for (int j=0;j<2;j++) {
    System.out.print(num[i][j] + " ");
	}
	System.out.println();
}
```
5. Printing Array column by column
```
for(int i=0;i<2;i++) {
  for (int j=0;j<2;j++) {
    System.out.print(num[j][i]+ " ");
	}
	System.out.println();
}
```
6. Printing Arrays using toString() method.
```
System.out.println(Arrays.toString(num));
```
It will Print the Array but not in the string representation means it will only print the reference of the arrays.
7. Printing Arrays in string representation using deepToString() method.
```
System.out.println(Arrays.deepToString(num));
```
It will print all the array.
