# ECE-2112-PA-1
Miguel Joaquin T. Cariño 2 ECE-D
# A. Word Rotation Problem
## OBJECTIVE:
The objective of this problem is to create a function that accepts a non-empty string which is named as rotate_word(). The function should be able to move the first character into the end of the given word while the rest of the remaining characters remain at their order as well as their capitalization. 
## DISCUSSIONS OF METHODS AND FUNCTIONS:
The function was defined as follows:
```python
def rotate_word(text):
    return text[1:]+text[0]
```
This function utilizes string slicing. In which text[1:] refers to getting all the characters starting from the second character, while text[0] gets the first character. Once the function is executed, these two are combined, making the first character appear at the end of all the remaining characters while retaining its capitalization. 
## Examples Given:
Example A1:
```python
rotate_word("python")
```
Returns:
```python
"ythonp"
```
Example A2:
```python
rotate_word("logic")
```
Returns:
```python
"ogicl"
```
Example A3:
```python
rotate_word("Code")
```
Returns:
```python
"odeC"
```
Example A4:
```python
rotate_word("A")
```
Returns:
```python
"A"
```
# B. Username Builder Problem
## OBJECTIVE
The objective of this problem is to create a function that is able to generate a username using a person's first and last name. Combining these two unique names while converting it to lowercase and separating them with a period. 
## DISCUSSIONS OF METHODS AND FUNCTIONS:
The functions was defined as follows:
```python
def make_username(firstname, lastname):
    return firstname.lower().replace(" ", "") + "." + lastname.lower().replace(" ", "")
```
The function utilizes string concatenation in order to combine the two lowercase names with a period in between them. The lower() is used in order to convert the names into lowercase characters. Which is then followed by .replace(" ", "") in order to remove the spaces in the names. 
## Examples Given:
Example B1:
```python
make_username("Ada", "Lovelace")
```
Returns:
```python
"ada.lovelace"
```
Example B2:
```python
make_username("Alan", "Turing")
```
Returns:
```python
"alan.turing"
```
Example B3:
```python
make_username("Ana Maria", "De Leon")
```
Returns:
```python
"anamaria.deleon"
```
# C. Bookend Swap Problem
## OBJECTIVE
The objective of this problem is to create a function that is able to swap the first and last elements of a sequence while keeping all the elements in between in their original order. 
## DISCUSSION OF METHODS AND FUNCTIONS:
The function was defined as follows:
```python
def swap_bookends(item):
    first, *middle, last = item
    return [last] + [*middle] + [first]
```
The function utilizes extended sequence unpacking in which *middle unpacks multiple element placed as the middle variable throughout the sequence. The first and last elements are identified using item[0] and item[-1], while item[1:-1] obtains all the elements between them. Once executed the function then returns the list in which the first and last elements are swapped while the middle elements retain it's order. 
## Examples Given:
Example C1:
```python
swap_bookends([1, 2, 3, 4, 5, 6,])
```
Returns:
```python
[6, 2, 3, 4, 5, 1]
```
Example C2:
```python
swap_bookends(["red", "green", "blue"])
```
Returns:
```python
["blue", "green", "blue"]
```
Example C3:
```python
swap_bookends([8, 3])
```
Returns:
```python
[3, 8]
```

Version histor



