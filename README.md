## Print Statements
> Python
```python
print("Hello World")
print("Hello {}".format(name))
```
> Java
```java
System.out.println("Hello World")
System.out.println("Hello "+ name)
System.out.printf("Hello World")
System.out.printf("Hello %s",name)
```
## Taking Input
> Python
```python
name = input("Enter your name")
```
```python
name = input()
```
```python
number = int(input())
```
```python
string_array = input().split(" ")
```
```python
int_array = list(map(int, input().split(" ")))
```
> Java
```java
// Define Object
 DataIntputStream din = new DataInputStream(System.in);
```
```java
// String as input
System.out.println("Enter your name");
String name = din.readLine();
```
```java
// Integer as input
Integer number = Integer.parseInt(din.readLine());
```
```java
// String array as input
String  string_array[] =  din.readLine().split("\\s");
```
```java
// Integer array as input
String  string_array[] =  din.readLine().split("\\s");
List<Integer> int_array =  new  ArrayList<Integer>();
for(String s:arr){
arr2.add(Integer.parseInt(s));
}
```
## for loop
> Python
```python
mylist = ["Mango","Apple","Orange"]
for i in mylist:
	print(i)
```
> Java
```java
String fruits[] = {"Mango","Apple","Orange"}
for(String f:fruits){
System.out.println(f);
}
```
## List
#### Adding Elements to list
> Python
```python
fruits= []
fruits.append("Mango")
fruits.append("Apple")
fruits.append("Orange")
```
> Java
```java
List<String> fruits= new ArrayList<String>();
fruits.add("Mango");
fruits.add("Apple");
fruits.add("Orange");
```
#### Access elements by index
> Python
```python
print(fruits[0])
```
> Java
```java
System.out.println(fruits.get(0));
```
#### Get Index of element
> Python
```python
fruits.index("Mango")
```
> Java
```java
fruits.indexOf("Mango");
```
#### Remove element from list by value
> Python
```python
fruits.remove("Mango")
# remove Integer value
fruits.remove(34)
```
> Java
```java
fruits.remove("Mango");
//remove Integer value
fruits.remove(new Integer(34));
```
#### Remove element from list by index
> Python
```python
del fruits[0]
```
> Java
```java
fruits.remove(0)
```
#### Get size of list
> Python
```python
len(fruits)
```
> Java
```java
fruits.size()
```
#### Iterate over list
> Python
```python
for element in list:
	print(element)
```
> Java
```java
Iterator<String> itr = fruits.iterator();
while(itr.hasNext()){
System.out.println(itr.next());
}
```
```java
for(String f:fruits){
System.out.println(f);
}
```
## Dictionary 
#### Adding elements
> Python
```python
users = {}
users["John"] = 3011
users["Joshua"] = 3012
users["Bill"] = 3013
```
> Java
```java
Map<String,Integer> users = new HashMap<String,Integer>();
users.put("John", 3011);
users.put("Joshua", 3012);
users.put("Bill", 3013);
```
#### Accessing Elements
> Python
```python
users["John"]
```
> Java
```java
users.get("John");
```
#### Remove elements from dictionary
> Python
```python
del users["Bill"]
```
> Java
```java
users.remove("Bill");
```
#### Get size of dictionary
> Python
```python
len(users)
```
> Java
```java
users.size();
```
#### Iterating over dictionary
> Python
```python
for key in users.keys():
	print(key,"=>",users[key])
```
```python
for value in users.values():
	print(value)
```
> Java
```java
for(String key : users.keySet()){
	System.out.println(users.get(key));
}
```
```java
for(int key : users.values()){
	System.out.println(key);
}
```
## Sort Elements
> Python
```python
numbers = [73, 8, 52, 12, 66, 31]
numbers.sort()
```
> Java
```java
Integer numbers[] = {73, 8, 52, 12, 66, 31};
Arrays.sort(numbers);
//Arrays.sort(numbers, Collections.reverseOrder());
```
```java
List<Integer> numbers = new ArrayList<Integer>();
numbers.add(73);
numbers.add(8);
numbers.add(52);
numbers.add(12);
numbers.add(66);
numbers.add(31);
Collections.sort(numbers);
//Collections.sort(numbers, Collections.reverseOrder());
```
