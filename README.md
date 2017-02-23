# UI-Code-Review
User Interface Code Review guidelines, suggestions and best practices

Javascript is a dynamically typed language which leaves code reviewers with bigger responsibilites. When it comes to code quality tools, the options are very less for javascript, which makes the situation worse. 

Here are few guidelines to help the review process more efficient.

Readability

1. A line should not contain more than 80 characters.
2. Follow proper indentation.
3. Methods/functions should not be too long.
4. Meaningful names for variables and functions instead of a, b or c.
5. Check if the code is understandable without having to rely on comments.

Maintainability:

1. No aribitray constants. [e.g height = height + 30 +'px', use a constants instead var heightAdjustment = 30;]
2. Are the methods extendable in future, be cautious about over-engineering


Runtime Vulnerability

1. While dealing with dynamically rendered elements, check for the element before applying styles.
2. Missing NULL checks, also try not to complicate null checks. [e.g if(variable == null), instead use if(variable)]

Aggressive Alarms

1. Avoid EVALs
2. No GLOBAL VARIABLES

Passive Alarms

1. Dead, Duplicate or Commented code
2. Unused imports
3. 
