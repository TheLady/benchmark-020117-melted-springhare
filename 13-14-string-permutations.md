### 14: String Permutations

Prints all of the permutations of the unique characters of an input string. For example, the permutation of the word "bar" would print the following:

```
bar
bra
abr
arb
rba
rab
```


### Strategy

pattern 1
return value of index [1],[2],[3] and pop [1] to back of stack
bar
arb
rba

pattern 2
reverse the permutations of those strings 
check to see if those permutations exist
console.log the permutations that aren't in the previous list of arrays

rab
  does rab permutation exist?
  no
  return rab

bra 
  does rab permutation exist?
  no
  return bra

arb
  does arb permutation exist?
  yes

repeat



### Code