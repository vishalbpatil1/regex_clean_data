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

Determining Data Quality
Is The Data Valid? (Validity)
The validity of your data is the degree to which it follows the rules of your particular requirements. For example, you how to import phone numbers of different customers, but in some places, you added email addresses in the data. Now because your needs were explicitly for phone numbers, the email addresses would be invalid. 

Validity errors take place when the input method isn’t properly inspected. You might be using spreadsheets for collecting your data. And you might enter the wrong information in the cells of the spreadsheet. 

There are multiple kinds of constraints your data has to conform to for being valid. Here they are:

Range: 

Some types of numbers have to be in a specific range. For example, the number of products you can transport in a day must have a minimum and maximum value. There would surely be a particular range for the data. There would be a starting point and an end-point. 

Data-Type: 

Some data cells might require a specific kind of data, such as numeric, Boolean, etc. For example, in a Boolean section, you wouldn’t add a numerical value.

Compulsory constraints:

In every scenario, there are some mandatory constraints your data should follow. The compulsory restrictions depend on your specific needs. Surely, specific columns of your data shouldn’t be empty.For example, in the list of your clients’ names, the column of ‘name’ can’t be empty. 

Cross-field examination:

There are certain conditions which affect multiple fields of data in a particular form. Suppose the time of departure of a flight couldn’t be earlier than it’s arrival. In a balance sheet, the sum of the debit and credit of the client must be the same. It can’t be different. 

These values are related to each other, and that’s why you might need to perform cross-field examination. 

Unique Requirements:

Particulars types of data have unique restrictions. Two customers can’t have the same customer support ticket. Such kind of data must be unique to a particular field and can’t be shared by multiple ones. 

Set-Membership Restrictions:

Some values are restricted to a particular set. Like, gender can either be Male, Female or Unknown. 

Regular Patterns:

Some pieces of data follow a specific format. For example, email addresses have the format ‘randomperson@randomemail.com’. Similarly, phone numbers have ten digits.

If the data isn’t in the required format, it would also be invalid. 

If a person omits the ‘@’ while entering an email address, then the email address would be invalid, wouldn’t it? Checking the validity of your data is the first step to determine its quality. Most of the time, the cause of entry of invalid information is human error.

Getting rid of it will help you in streamlining your process and avoiding useless data values beforehand. 

Data Science Advanced Certification, 250+ Hiring Partners, 300+ Hours of Learning, 0% EMI

Accuracy
Now that you know that most of the data you have is valid, you’ll have to focus on establishing its accuracy. Even though the data is valid, it doesn’t mean the data is accurate. And determining accuracy helps you to figure out if the data you entered was accurate or not. 

The address of a client could be in the right format, but it doesn’t need to be the right one. Maybe the email has an additional digit or character that makes it wrong. Another example is of the phone number of a customer. 
