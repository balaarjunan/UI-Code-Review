# UI-Code-Review
User Interface Code Review guidelines, suggestions and best practices

Javascript is a dynamically typed language which leaves code reviewers with bigger responsibilities. When it comes to code quality tools, the options are very less for javascript, which makes the situation worse. 

Here are few guidelines to help the review process more efficient. The review is themed around the concept of PURE.


Performant

1. While dealing with dynamically rendered elements, check for the element before applying styles.
2. Missing NULL checks, also try not to complicate null checks. [e.g if(variable == null), instead use if(variable)]
3. Performance pitfalls like loops, DOM manipulations, lack of caching where required
4. Avoid EVALs
5. No GLOBAL VARIABLES
6. Dead, Duplicate or Commented code
7. Unused imports

Unit Testable

1. Is the code Unit-testable
2. Could it be Unit tested with minimal mock data.

Readability

1. A line should not contain more than 80 characters.
2. Follow proper indentation.
3. Methods/functions should not be too long.
4. Meaningful names for variables and functions instead of a, b or c.
5. Check if the code is understandable without having to rely on comments.
6. Emphasis semi-colon;
7. Loops should always have parenthesis. 

Extendable

1. No arbitrary constants. [e.g height = height + 30 +'px', use a constants instead var heightAdjustment = 30;]
2. Are the methods extendable in future, be cautious about over-engineering





