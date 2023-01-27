# CSE 15L Lab Report 2 Ayan Gaur

## *Part 1 - StringServer:*

For creating StringServer, we must create a Server.java file which contained the code for creating a web server using Java's built in Http-Server.
Next, we must create a StringServer.java file which contained the functionality to keep track of a single string that gets added to by incoming requests.

The StringServer.java file looks like this:

<img width="1296" alt="Screenshot 2023-01-26 at 9 45 10 PM" src="https://user-images.githubusercontent.com/122495485/215018146-35e6e58f-d93e-4242-934d-1729ff3c13b1.png">

The Server.java file looks like this:

<img width="945" alt="Screenshot 2023-01-26 at 9 46 59 PM" src="https://user-images.githubusercontent.com/122495485/215018262-baa6c129-4389-4fae-8df6-104152ca36f2.png">

To use the StringServer, we have to first compile both the files using `javac Server.java StringServer.java`. After this files have been compiled we can run them using `java StringServer 4000`. Any number between 1024 and 49151 will work, using 4000 is not a compulsion.

The web server can be launched now, and should look like this:

<img width="253" alt="Screenshot 2023-01-26 at 10 09 12 PM" src="https://user-images.githubusercontent.com/122495485/215020905-eaa7ab71-2fbc-4812-912e-de66accb9ccc.png">

Using `localhost:4000/add-message?s=<String>` Strings can be added. The web server should now be,

<img width="408" alt="Screenshot 2023-01-26 at 10 09 58 PM" src="https://user-images.githubusercontent.com/122495485/215020992-7d09af26-cad7-48b2-9ddd-631be323d91b.png">

We can add another string, and it should look like this:

<img width="452" alt="Screenshot 2023-01-26 at 10 10 24 PM" src="https://user-images.githubusercontent.com/122495485/215021053-d289b30a-1da8-4585-bab3-19b0520b8ae9.png">

For both screenshots, after the server has been started and the URL is opened, the handleRequest method is used. The string checks if there is anything after the forward slash. If the add-message arguement is present, the text after it is split by the `=`. Then the query present after the `=` is added to an arraylist and returned as a string, which has been formatted to put every element in a new line. 

If a different number is used in the URL suddenly, it will not work, the server must be started with the number it is to be used with. If we remove the add-message query it will show us just the previously added elements. Instead of putting words and letters as values, we can also put numbers. The method recognizes the numbers as Strings and will display it the same way.

## *Part 2 - Bugs:*

For ArrayExamples.java `reverseInPlace()` method.

1. Failure inducing input for JUnit:
```
public class ArrayTests {
	@Test 
	public void testReverseInPlace() {
    int[] input1 = {1, 2, 3, 4};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{4, 3, 2, 1}, input1);
	}
```

2. Non-failure inducing input for JUnit:
```
public class ArrayTests {
	@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
  ```
  
3. Symptom:

![MT8BIQG-9jljAQevrJg6JD-C1_DqPPbkd-kteGfkENhaOvF8-MwD_BW4ssmnmQbQLp2mHUk87VvM1zyKuG08eH43zFecpNS8-9xAqlIkrN6JMsmwzgrKvsOo1m9-](https://user-images.githubusercontent.com/122495485/215024152-a42e76d0-dd1b-437a-a510-c715474e3069.png)

The second test, does not have a symptom since the test passes.

<img width="439" alt="Screenshot 2023-01-26 at 10 38 15 PM" src="https://user-images.githubusercontent.com/122495485/215024667-a7b21679-da42-48b6-8e7f-a5b5ec132911.png">

4. Bug:

Before:
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
After:
```
  static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int currArr = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length-1-i] = currArr;
    }
  }
  ```
This would fix the bug since before this the values of the elements in the first half of the array are changed to the latter half, but after the mid-point it uses those changed values to replace the values of the second half of the array, hence not making any change to the second half.

## *Part 3 - New Learnings:*

1. I learnt about using Java to create web servers which can be run locally, and how to use the query provided to the server to display different things.

2. I learnt how particular you have to be while testing and debugging code, and how you have to go through every possible set of inputs to check the code.
