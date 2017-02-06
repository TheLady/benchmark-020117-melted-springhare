### 12: String Me Along

Given an input string, print the longest substring that contains a maximum of two unique characters.

If there are multiple substrings that qualify as 'longest', print substring that is furthest to the right.

**Examples:**

```
ghhiiii -> hhiiii

efgefghiiikk -> iiikk
```


### Strategy
a substring can't be the whole string

binary search? node?

start at the right
is the current index value the same as the value of the previous index? 
yes 
keep going

  is that previous index value the same its previous index?
no 
keep going

is that previous index value the same its previous index?   
yes 
keep going (1 match)

is the previous index value the same its previous index? 
yes (2 matches)

keep going

previous index value the same its previous index? 
yes (3 matches)

stop 
calculate the length from the previous index to the end of the string
push that into an array (substring1)
delete from string



Option 2
Search for patterns instead of values
 https://en.wikipedia.org/wiki/Regular_expression

look at javascript lastIndex

skipping this one



### Code