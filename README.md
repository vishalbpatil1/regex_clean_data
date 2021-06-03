# regex_clean_data
Text preprocessing is one of the most important tasks in Natural Language Processing (NLP). For instance, you may want to remove all punctuation marks from text documents before they can be used for text classification. Similarly, you may want to extract numbers from a text string. Writing manual scripts for such preprocessing tasks requires a lot of effort and is prone to errors. Keeping in view the importance of these preprocessing tasks, the Regular Expressions (aka Regex) have been developed in different languages in order to ease these text preprocessing tasks.

# Conclusion
In this repo we studied some of the most commonly used regex functions in Python. Regular expressions are extremely useful for preprocessing text that can be further used for a variety of applications, such as topic modeling, text classification, sentimental analysis, and text summarization, etc.

# imp
```bash
## Metacharacters are characters with a special meaning:
[]  A set of characters       "[a-m]"

\   Signals a special sequence (can also be used to escape special characters)  "\d"

.   Any character (except newline character)    "he..o"

^   Starts with "^hello"


$   Ends with   "world$"

*   Zero or more occurrences    "aix*"

+   One or more occurrences "aix+"

{}  Exactly the specified number of occurrences "al{2}"


|   Either or   "falls|stays"

()  Capture and group
[^arn]  Returns a match for any character EXCEPT a, r, and n


[0123]  Returns a match where any of the specified digits (0, 1, 2, or 3) are present


[0-9]   Returns a match for any digit between 0 and 9

[0-5][0-9]  Returns a match for any two-digit numbers from 00 and 59

[a-zA-Z]    Returns a match for any character alphabetically between a and z, lower case OR upper case


[+] In sets, +, *, ., |, (), $,{} has no special meaning, so [+] means: return a match for any + character in the string
```
