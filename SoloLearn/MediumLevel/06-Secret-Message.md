# Secret Message 
## Objective
 
You are trying to send a secret message, and you've decided to encode it by replacing every letter in your message with its corresponding letter in a backwards version of the alphabet.  
What do your messages look like? 
 

## Task:  

Create a program that replaces each letter in a message with its corresponding letter in a backwards version of the English alphabet. 
 

## Input Format:  

A string of your message in its normal form. 
 

## Output Format:  

A string of your message once you have encoded it (all lower case). 
 

## Sample Input:  

```
Hello World 
```
 

## Sample Output:  

```
svool dliow 
```


## Explanation:  

If you replace each letter in 'Hello World' with the corresponding letter in a backwards version of the alphabet, you get 'svool dliow'.


## Solution

```python

alphabet='abcdefghijklmnopqrstuvwxyz'
secret_message=input().lower()

new_word=[]
for word in secret_message:
    if word == ' ':
        new_word.append(' ')
    else:
        new_word.append(alphabet[::-1][alphabet.index(word)])

print(''.join(new_word))

```


---