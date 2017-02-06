### 13: Braille

Your goal is to read in a string of Braille characters (definition [here](https://en.wikipedia.org/wiki/English_Braille#Alphabet)) and translate the word to standard English letters (you can ignore any special characters, including spaces).

A lowered bump is a dot ('.'), and a raised bump is an upper-case 'O' character.


**Example Input:**

```
O. O. O. O. O. .O O. O. O. OO
OO .O O. O. .O OO .O OO O. .O
.. .. O. O. O. .O O. O. O. ..
```

**Example Output:**

```
helloworld
```

### Strategy
write out each braille character in 0.

make each braille character a string and assign it a variable that is a letter

make letter-braille key-value base 6 or base 2 notation - do I define a letter or define a dot

make it a base 10 number (because it's easier for humans to understand)

stretch - write a function to automate the matching of key-value pair/ generate key-value pair w a function

output each letter



  



###Code