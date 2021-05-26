## Lecture Notes

### Data types:
* Integers - `int`
* Floating-point numbers - `float` - NaN belongs to this group
* Strings - `str`
* Booleans - `bool` - two values: True and False.
* Lists - `list`
* Tuples - `tuple`
* Sets - `set`
* Dictionaries - `dict`

### Summary

|Data Structure	| Preserves order | Mutable | Symbol| Can contain duplicates | Can be sliced |
|---------|------|------|------|------|------|
|str	|✓	|☓	|''or""|	✓|✓|
|list	|✓	|✓	|[] |	✓|✓|
|tuple	|✓	|☓	|() |	✓|✓|
|set	|☓	|✓	|{} |	☓|☓|
|dict  |✓	|✓	|{} | 	☓| ☓|

### Formatting Dates: More on <code>strftime()</code> and <code>strptime()</code>

<code>strptime()</code> is the method we used before, and you’ll recall that it can turn a date and time that’s formatted as a text string into a datetime object, in the following format:

<code>time.strptime(string, format)</code>

Note that it takes two arguments:

<code>string</code> − the time in string format that we want to convert

<code>format</code> − the specific formatting of the time in the string, so that <code>strptime()</code> can parse it correctly

#### Below is a list of directives used in <code>strftime()</code> and their meanings
| Directive | Meaning|
|-----------|--------|
| %a |Weekday abb. Sun, Mon, …, Sat (en_US)|
| %A | Weekday Full Sunday,Monday (en_US)|
| %w | weekday as decimal 0,1,2,3.. |
| %d | day of month as decimal 0,1,2,...30 ||
| %b | Month Jan, Feb, …, Dec (en_US) |
| %B | Month January,February... |
| %m | Month as a zero-padded decimal |
| %y | Year without century as zero padded decimal 00,01,..,99 |
| %Y | Year with century 1970,1980 etc. |
| %H | our (24-hour clock) as a zero-padded decimal number.00, 01, …, 23 |
| %I | Hour (12-hour clock) as a zero-padded decimal number.01, 02, …, 12 |
| %p | Am,PM |
| %M | Minute 00,01..,59 |
| %S | Second 00,01..,59 |

Check for Masters material: https://www.tomasbeuzen.com/