### 9: Parens-B-Gone

`(((7)))` is an expression that contains too many parentheses.

How many is "too many" parentheses?

If you can strip the expression of one set of parentheses, and the same expression still contains parentheses, it has too many parentheses.

In the above example, `(7)` would be the proper stripping of parentheses.

**Example Inputs:**
```
((1((23)(45)))6)  

(((1234)(((5)67))))

12((3))
```

**Example Outputs:**
```
((1((23)(45)))6)  

((1234)((5)67))

12(3)
```

### Strategy
<!-- translate parentheses into binary values   -->

remove paren if [0] == ( and index value at the end of the array is )
and if index at [1] and the value at [last index - 1] is ) delete [0] and [index value at end of array]

make the input a string (including parens)
Count number of parens at end of input
Count number of parens at beginning of input

if countFrontEnd===countBackEnd delete paren at index[0] and [lastIndex]





###Code