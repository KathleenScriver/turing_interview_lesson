# `#each` Review
(30 min)

What to cover:

- identify parts of our enumerable
    - block, block variable
- Naming conventions, what should we name our block variable?

- return vale of #each

- what do we need if we want to hold on to or save the transformation we're doing or keep track of what we're counting, etc. Basically, when we want to get something back and not just have side effects. 
    - Display with an example. If we just want to puts something, we're not really concerned with the data after we've puts-ed it, we just want the side-effect of puts-ing! For example, if I have a list of cat names, and I only want back the names that are 5 characters are shorter, how do I keep track of these if #each returns the original array?

- Quick practice to take a pulse on the class (they do)
    - given array of numbers, how can I use #each to add all these numbers together?

What questions do you have?

- If we're chuggin along:
    - What if I have a Cat class with a name attribute, exposed as a method with attr_reader. I have an array of Cat instances. How can I get each cat's name?