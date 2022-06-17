# Email Address Regex Tutorial

This will be a brief regex tutorial for matching an email address. The regex for this is as follows: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary

Matching an email address in regex looks like the following: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
</br>
Simply put, we need to match 3 parts- everything before '@', everything after the '@' but before the '.' and everything after the '.'

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

### Anchors
The anchors are the ^ and $ symbols. The ^ marks the beginning of your string of characters and the $ marks the end.
</br>
The \ is used to mark a special 'escaped' character. In our regex example above, the \ is used to tell us that the '.' is meant to be interpreted as a '.' instead of a 'match any character' operator.

### Quantifiers
The quantifiers let us know the lower and upper bounds of how many characters we can accept. In our regex above, quantifiers are the {2,6} after the '.' which lets us know we can accept 2-6 characters such as .uk or .com

### Character Classes
A Character Class or Character set is what we see enclosed in [ ] above. This lets us know we can accept any character inside of the brackets. In our case, we can accept any lower case letter, any digit, and certain special characters.

### Flags
Regex flags allow us to bend the rules while we are searching for a match. This would be something like making our search case insensitive or making a sticky search to only search part of the string from one point forward.

### Grouping and Capturing
We use parentheses to group elements in our regex. For matching an email, we can break it down into separate parts to make it easier to search:
</br>
(lonny)@(example).(com)

### Bracket Expressions
Anything that you want to match must be enclosed in [ ]. Any characters specified in the brackets tell us what characters are allowed for that specific component of the regex.

### Greedy and Lazy Match
The '+' is a greedy operator. This tells us that we can match more than one of character like the two "n's" in my name:
</br>
(lonny)@(example).(com)

## Author
My name is Lonny Vandenberg. I am finishing my Full Stack Web Development course at University of Utah. Check out my GitHub: [lonny-v](https://github.com/lonny-v)
