
# Matching an Email -- REGEX Tutorial

#### Summary
Regular expressions are patterns used to match character combinations in strings. In JavaScript, regular expressions are also objects.

Used to verify a valid email address:
(  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ )



## Table of Contents

### Anchors

We start by using this " ^ ". This anchor simply just means the beginning.

rest of anchors are below:

##### Beginning: 
Matches the beginning of the string, or the beginning of a line if the multiline flag (m) is enabled. This matches a position, not a character.
ex: " ^\w+ ", 

##### end: 
Matches the specified quantity of the previous token. {1,3} will match 1 to 3. {3} will match exactly 3. {3,} will match 3 or more.
ex: "b\w{2,3}"

##### word boundary: 
Matches a word boundary position between a word character and non-word character or position (start / end of string).
ex: " s\b "

##### not word boundary:
Matches any position that is not a word boundary. This matches a position, not a character.
ex: " s\B "

### Quantifiers:

Match between 2 and 3 of the preceding token.
ex: " {2,3} "


##### OR Operator:

Acts like a boolean OR. Matches the expression before or after the |.
It can operate within a group, or on a whole expression. The patterns will be tested in order.
ex: " b(a | e | i)d "

##### Character Classes:



##### Flags:

After the ending /, you can add g (global search), i(case-sensitive search), or m(mult-line search) as optional flags.

##### Grouping and Capturing:

Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.

It uses this " ( "

##### Bracket Expressions

[a-z0-9_\.-]
[\da-z\.-] 
[a-z\.]


##### Greedy and Lazy Match

Makes the preceding quantifier lazy, causing it to match as few characters as possible. By default, quantifiers are greedy, and will match as many characters as possible.



##### Boundaries
##### Back-references
##### Look-ahead and Look-behind
##### Regex Components

Author
Sky