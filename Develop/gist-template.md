# RegexForDummies


First of all, thanks for choosing my professional walkthrough on what regular expressions are, in this article I will teach you all you need to know as if you had to pass an exam on regular expressions. Please be patient as I can only make this article as "Dummy" friendly as I can.

## Summary
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

You see that? Thats a regular expression. To a developer, they might be able to see that its a criteria for things such as passwords or usernames or even an email. However, to a John Doe, you'll think its some code out of a movie "Hacking a database" scene. Regex is simplier than it looks, In this particular sample, it is a formula for creating an email. Further on in this article, Ill breakdown exactly what each part means in sections to make it easier to read.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)


## Regex Components

### Anchors
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

There are two anchors in this particular regex, "^" and "$" . The ^ signals the start of the criteria. in other words, "Your email must begin with one of the following...". The $ in my opinion couldve been done a different way but what is means is the opposite, "Your email must end with the following..." If you notice, in the sample regex, it has a "@" in the middle of it, its pretty self explanitory even for dummies what comes before and after that in an email. 
### Quantifiers
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

A quantifier should really just be renamed "Max and Min" because thats really all it is. In this example, you can see "{2,6}" at the end right before the $ anchor. that means that after the . in the email, the minimum amount of characters is 2 and the maximum is 6. Again this is another concept thats easier than it seems.
### Flags
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

One thing thats cool to mention to any non-dummy geeks out there is the functionality of flags, this particular expression doesnt have any flags but what flags are is additional requirements such as seeing if there are any matching emails that already exist or also a case-insensitive search. These come at the very end of the whole regex(regular expression) after the last /. 
### Grouping and Capturing
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This section in my opinion is very "essential" and is a basic concept to know before diving into regular expressions. In our regex, you see multiple (parenthesis), this is called subexpressions. its just a way to seperate the requirements of the regex. In our example, "([a-z0-9_\.-]+)" is the start of the email or anything before the "@" , ([\da-z\.-]+) is anything after the @, this is usually the "google or yahoo" and "([a-z\.]{2,6})" is the final ".com" or whatever you need to put down.
### Bracket Expressions
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Please remember from our "Grouping and Capturing" section, Inside of our subexpressions, we also have Brackets "[]". these brackets are too simple to explain. They just tell us th=e things we want to include in our email. in our regex, "([a-z0-9_\.-]+)" the braket expressions [a-z0-9_\.-] just mean that we want these in our email, letters from a-z, numbers from 0-9, underscores, backslashes, periods, and dashes. 
### Boundaries
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

If regex had families, an anchor would be a boundaries sibling, essentially theyre the same thing. There is an article in which I love how the author wrote it out. "Assert that immediately to the left of the current position, we can find the left wall, while to the right of the current position we cannot find the left wall." This is in reference to the ^ and $ anchors. a boundarie is basically putting the regular expression into a glass container, Just for format and reading purposes.

## Author

My names Daniel Cruz, I am a devoted 'learner' and love to outsource all my learning material and compile it all into an organized notes layout, making it easy to read as if I were to sell my notes. Doing that has really helped me grasp many concepts in many areas and is something I recommend to anyone. Apart from having a love for learning, Im a pretty real and considerate person which explains why I went out the way to outsource my information from various different articles and compile it all into one for the readers benefit, considering the reader is a "dummy" to tech. 

Attached below are my contact information:

Github Username : DACZuniga

Email : Danielcruz.34776@gmail.com

Profile URL : https://github.com/Daczuniga


REFERENCES :

https://www.rexegg.com/regex-boundaries.html - REXEGG "The World's Most tyrannosaurical regex tutorial"