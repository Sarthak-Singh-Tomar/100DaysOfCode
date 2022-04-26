# Day1:

## Wrapper Class
1. Wrapper Class: A Wrapper class is a class whose object wraps or contains primitive data types. When we create an object to a wrapper class, it contains a field and in this field, we can store primitive data types. In other words, we can wrap a primitive value into a wrapper class object.
2. AutoBoxing: Automatic conversion of primitive types to the object of their corresponding wrapper classes is known as autoboxing.
3. UnBoxing:  It is just the reverse process of autoboxing. Automatically converting an object of a wrapper class to its corresponding primitive type is known as unboxing.

## ArrayList in Java
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
