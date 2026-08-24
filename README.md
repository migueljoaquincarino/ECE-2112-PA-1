# ECE-2112-PA-1
Miguel Joaquin T. Cariño 2 ECE-D
# A. Word Rotation Problem
## OBJECTIVE:
The objective of this problem is to create a function that accepts a non-empty string which is named as rotate_word(). The function should be able to move the first character into the end of the given word while the rest of the remaining characters remain at their order as well as their capitalization. 
## DISCUSSIONS OF METHODS AND FUNCTIONS:
The function was defined as follows:
```python
def rotate_word(text):
    text[1:]+text[0]
```
This function utilizes string slicing and string concatenation. In which text[1:] refers to getting all the characters starting from the second character, while text[0] gets the first character. Once the function is executed, these two are combined, making the first character appear at the end of all the remaining characters while retaining its capitalization. 
## Example Given:
```python
rotate_word("Miguel")
```
```python
"iguelM"
```
```python
rotate_word("eLectronics")
```
```python
"Lectronicse"
```
```python
rotate_word("coffee")
```
# B. Username Builder Problem
## OBJECTIVE

```python
"offeec"
```

