### 7: Who Wants A Date?

According to ISO 8601 standard, the best way to format a date is:

yyyy-mm-dd

Learners Guild's database has become corrupted with mixed up date formats.

They can come in *any* of the 6 formats below:

```
yyyy-mm-dd
mm/dd/yy
mm#yy#dd
dd*mm*yyyy
(month in words) dd, yy
(month in words) dd, yyyy
```

(month in words) can be:

```Jan Feb Mar Apr May Jun Jul Aug Sep Oct Nov Dec```

Years are restricted to ```1950-2049```.

**Input:**

The 1000 dates in [this gist](https://gist.github.com/deonna/d2800f6301d326979b3a71da8cf0cb8f).

**Output:**

All the dates in the `yyyy-mm-dd` ISO 8601 standard date format.

---

### Strategy

result attributes (create a prototype)

construct year 
number with values
 no upper limit
 lower limit is 1900 (or base it on the world's oldest person)

identify whether date objects are letters, numbers, spaces, #'s, *'s, /'s, dashes,

in each date
 identify location of date characters in relation to -'s
 identify location of date characters in relation to /'s
 identify location of date characters in relation to *'s
 identify location of date characters in relation to #'s
 identify location of date characters in relation to 's
 etc.

 handle this case "1991-01-21" vs 06*04*1965 order

write functions that identify each date pattern
  find each date with that pattern and make it into a dictionary/array 

if date is in ___ format, apply (some function) 
if date is in ___ format, apply (some other function)




###Code
