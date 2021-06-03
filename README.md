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

Data Cleansing Techniques
Your choice of data cleaning techniques relies on a lot of factors. First, what kind of data are you dealing with? Are they numeric values or strings? Unless you have too few values to handle, you shouldn’t expect to clean your data with just one technique as well.

You might need to use multiple techniques for a better result. The more data types you have to handle, the more cleansing techniques you’ll have to use. Being familiar with all of these methods will help you in rectifying errors and getting rid of useless data. 

1. Remove Irrelevant Values
The first and foremost thing you should do is remove useless pieces of data from your system. Any useless or irrelevant data is the one you don’t need. It might not fit the context of your issue. 

You might only have to measure the average age of your sales staff. Then their email address wouldn’t be required. Another example is you might be checking to see how many customers you contacted in a month. In this case, you wouldn’t need the data of people you reached in a prior month.

However, before you remove a particular piece of data, make sure that it is irrelevant because you might need it to check its correlated values later on (for checking the consistency). And if you can get a second opinion from a more experienced expert before removing data, feel free to do so. 

You wouldn’t want to delete some values and regret the decision later on. But once you’re assured that the data is irrelevant, get rid of it. 

2. Get Rid of Duplicate Values
Duplicates are similar to useless values – You don’t need them. They only increase the amount of data you have and waste your time. You can get rid of them with simple searches. Duplicate values could be present in your system for several reasons.

Maybe you combined the data of multiple sources. Or, perhaps the person submitting the data repeated a value mistakingly. Some user clicked twice on ‘enter’ when they were filling an online form. You should remove the duplicates as soon as you find them. 

3. Avoid Typos (and similar errors)
Typos are a result of human error and can be present anywhere. You can fix typos through multiple algorithms and techniques. You can map the values and convert them into the correct spelling. Typos are essential to fix because models treat different values differently. Strings rely a lot on their spellings and cases.

‘George’ is different from ‘george’ even though they have the same spelling. Similarly ‘Mike’ and ‘Mice’ are different from each other, also though they have the same number of characters. You’ll need to look for typos such as this and fix them appropriately. 

Another error similar to typos is of strings’ size. You might need to pad them to keep them in the same format. For example, your dataset might require you to have 5-digit numbers only. So if you have any value which only has four digits such as ‘3994’ you can add a zero in the beginning to increase its number of digits.

Its value would remain the same as ‘03994’, but it’ll keep your data uniform. An additional error with strings is of white spaces. Make sure you remove them from your strings to keep them consistent. 

4. Convert Data Types
Data types should be uniform across your dataset. A string can’t be numeric nor can a numeric be a boolean. There are several things you should keep in mind when it comes to converting data types:

Keep numeric values as numerics
Check whether a numeric is a string or not. If you entered it as a string, it would be incorrect. 
If you can’t convert a specific data value, you should enter ‘NA value’ or something of this sort. Make sure you add a warning as well to show that this particular value is wrong.
5. Take Care of Missing Values
There would always be a piece of missing data. You can’t avoid it. So you should know how to handle them to keep your data clean and free from errors. A particular column in your dataset may have too many missing values. In that case, it would be wise to get rid of the entire column because it doesn’t have enough data to work with.

Point to note: You shouldn’t ignore missing values.

Ignoring missing values can be a significant mistake because they will contaminate your data, and you won’t get accurate results. There are multiple ways to deal with missing values. 

Imputing Missing Values:

You can impute missing values, which means, assuming the approximate value. You can use linear regression or median to calculate the missing value. However, this method has its implications because you can’t be sure if that would be the real value. 

Another method to impute missing values is to copy the data from a similar dataset. This method is called ‘Hot-deck imputation’. You’re adding value in your current record while considering some constraints such as data-type and range. 

Highlighting Missing Values:

Imputation isn’t always the best measure to take care of missing values. Many experts argue that it only leads to more mixed results as they are not ‘real’. So, you can take another approach and inform the model that the data is missing. Telling the model (or the algorithm) that the specific value is unavailable can be a piece of information as well. 
