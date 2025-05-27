# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python program that accepts a string and removes the character at a specified index.

## 🧠 Algorithm
1. Define a function named `remove` that takes the input string as an argument.
2. Read the index `n` from the user input.
3. Initialize an empty string `a` to store the new string.
4. Iterate over each index of the string using a `for` loop.
5. Check if the current index `i` is not equal to `n`.
6. If `i != n`, append the character at index `i` to string `a`.
7. After the loop, return the modified string `a`.
8. Print the final result.

## 💻 Program
~~~

def remove_character(string, index):
    if index < 0 or index >= len(string):
        return "Invalid index!"
    return string[:index] + string[index+1:]

user_string = input("Enter a string: ")
index_to_remove = int(input("Enter the index of the character to remove: "))

result = remove_character(user_string, index_to_remove)
print(f"\nString after removing character at index {index_to_remove}: {result}")
~~~
## Output
~~~
Enter a string: hello
Enter the index of the character to remove: 1

String after removing character at index 1: hllo
~~~

## Result
Thus given program is verified successfully.
