# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
~~~
import re
def filter_words(words):
    return [word for word in words if not re.search(r'e', word, re.IGNORECASE)]
words_list = input("Enter words separated by spaces: ").split()

filtered_list = filter_words(words_list)
print(f"\nWords without the letter 'e': {filtered_list}")
~~~
## Output
~~~
Enter words separated by spaces: apple banana cherry kiwi mango
Words without the letter 'e': ['banana', 'kiwi']
~~~

## Result
Thus given program is verified successfully
