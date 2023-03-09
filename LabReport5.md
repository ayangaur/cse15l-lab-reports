# CSE 15L Lab Report 5 Ayan Gaur

## Bash Script for Lab Report 4

In Lab Report 4, the fastest way to complete all the challenges would undoubtedly be a bash script. So I will use a bash script to complete all the steps from 4-9.

### 1. Original Method for Lab Report 4

Originally I just used the up arrow to navigate through commands in the history of the terminal and <tab> to autocomplete methods. Although this meant that I did not have to type out everything, it was still not that fast.

### 2. Bash Script
  
The bash script I created ran all the steps from 4-9.
```
#!/bin/bash

# Step 1: Clone the repository
git clone git@github.com:ayangaur/lab7.git
cd lab7

# Step 2: Compile the Java code and tests
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java

# Step 3: Run the JUnit tests
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests

# Step 4: Fix the Java code
# Edit the Java files in the src directory as necessary
sed -i '43s/index1 += 1/index2 += 1/g' ListExamples.java

# Step 5: Re-compile and verify that the JUnit tests pass
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests

# Step 6: Commit and push the changes back to GitHub
git add .
git commit -m "Fix Java code"
git push origin main
```
Now if we just run the bash script, it makes all the necessary changes and updates the ListExamples.java file and then updates the GitHub repository.

We get the following output:

<img width="731" alt="Screenshot 2023-03-09 at 3 37 08 PM" src="https://user-images.githubusercontent.com/122495485/224184816-cf8bc636-4b51-4eb2-a04c-60351f76ac68.png">

### 3. Other ways to complete the Lab Tasks
We have used ChatGPT quite a bit in labs. So I decided to ask ChatGPT to give me a quick method to complete these lab tasks.
<img width="827" alt="Screenshot 2023-03-09 at 3 45 24 PM" src="https://user-images.githubusercontent.com/122495485/224185933-67cea0cc-e429-446c-a4aa-3a8826b3601d.png">

The command given by ChatGPT just combines all the individual commands we ran using the `&&` symbol. This command also worked. Instead of using the `sed` command which can directly edit the needed line, this uses the `nano` command and we still have to make the needed changes by going to the required line.
  
<img width="951" alt="Screenshot 2023-03-09 at 3 50 30 PM" src="https://user-images.githubusercontent.com/122495485/224187296-3d875025-d044-492b-b8b4-a39f55e8ab29.png">

If I had to take part in the competition again I would probably use the single line command using the `&&` symbols, and the `sed -i` command to replace the old line with the new line in the java file. This would mean I would only have to perform two button pressed `<up> <enter>` and that would be it. (Probably should have tried this before, so I could've won :/)
