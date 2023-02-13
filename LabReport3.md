# CSE 15L Lab Report 3 Ayan Gaur

## grep

The `grep` command has many ways to use it. 
https://phoenixnap.com/kb/grep-command-linux-unix-examples shows various ways to use the grep command. Using this website I have picked the following extensions.

### 1. To find whole words
`grep -w` can be used to find whole words instead of just the specific pattern in the text file.

![Screenshot 2023-02-12 at 8 39 45 PM](https://user-images.githubusercontent.com/122495485/218372256-fda53456-4715-4960-a56b-9d0f02f87142.jpeg)

Only results from where the word India is used are shown and words like Indian which are contain India in them do not show up.

![Screenshot 2023-02-12 at 9 10 44 PM](https://user-images.githubusercontent.com/122495485/218375775-68ae3513-7332-48f3-add2-b4a3e3f88f8b.jpeg)


### 2. To search all subdirectories
`grep -r` can be used to search through all the subdirectories of a directory instead of having to check them individually.

![Screenshot 2023-02-12 at 8 43 57 PM](https://user-images.githubusercontent.com/122495485/218372542-767aecc7-0824-4f09-93d6-00b9a339e161.jpeg)

Using the `-r` extension, we went through all the subdirectories of `written_2`

![Screenshot 2023-02-12 at 9 08 11 PM](https://user-images.githubusercontent.com/122495485/218375578-73ba4e1a-17ac-4947-bef5-d841684397af.jpeg)


### 3. To search for both lowercase and uppercase
`grep -i` can be used to make the grep command search for the string, in both uppercase and lowercase.

![Screenshot 2023-02-12 at 8 50 15 PM](https://user-images.githubusercontent.com/122495485/218373346-7aa20302-cea2-429b-b681-ad68ab42590d.jpeg)

Over here even the lowercase results can be seen although the main string was 'Without'.

![Screenshot 2023-02-12 at 9 06 11 PM](https://user-images.githubusercontent.com/122495485/218375201-c3e51a33-849c-4404-b331-4b75a0321a6e.jpeg)


### 4. To Count the Number of Matches
`grep -c` can be used to get the number of times a string appears in a file.

![Screenshot 2023-02-12 at 9 02 53 PM](https://user-images.githubusercontent.com/122495485/218374791-c6d58d72-0d49-48b0-a4a5-991865f66d0b.jpeg)

The number of the occurences are displayed next to each filename.

![Screenshot 2023-02-12 at 9 04 08 PM](https://user-images.githubusercontent.com/122495485/218374931-c963be28-9818-40bb-8043-1f1111b74d87.jpeg)
