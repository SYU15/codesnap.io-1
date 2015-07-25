---
title: Writing high quality code
tags: best practices, javascript
published: true
---

You might think that writing high quality code means writing code that successfully solves the problem at hand in the fewest lines possible, as efficiently as possible. However, some engineers find that sacrificing brevity and possibly even efficiency (while still working within any time and space constraints) can actually be more effective. So then...

# what is high quality code?

decoupled 
well organized
well commented

# why is it important to write high quality code?

When working on large and complex applications, it is extremely important to keep your code organized. First, clearly organized code helps you maintain a clear mental model of the problem you're trying to solve. If you get stuck, looking back at your code should not induce a panic. 

Second, clearly organized code is readable. There is a saying that "you should write code for your future self". That is, you, your teammates, or anyone else who may need to review your code in the future should be able to easily understand what is going. 

Finally, a good structure will allow your code to be more easily maintained. If you need to come back and make changes, having code that is well organized and decoupled will significantly reduce the need for tedious debugging and refactoring. 

# three levels of separation: functional (length, naming), page, file

Now that we've discussed the benefits of well-organized and decoupled code, let's discuss some  actionable approaches to implementing these principles. Disclaimer: some of these notes are personal preference. There is often no "right" way to organize code, and the most appropriate approach will often depend on the project, the needs of the team, and the individual engineer's preferences. 

We will consider code organization from a three levels:

1. functional
  Function and variable names should be clear and impart the purpose of that code.
  Keep function bodies to no more than 10 lines
2. page
  Some engineers prefer to add a new file when the length of code on a page reaches the fold (the edge of what is readable without scrolling)
3. file structure
  organize by feature, not by type - this is how we usually work with code
  keep dependencies separate from app files
  write modularly and use dependency injection, when possible