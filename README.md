# `#each` Review
(~30 min)

## Objectives
1. Identify the parts of our enumerable
1. Demonstrate using `#each` when we just want side effects
1. Practice examples using `#each` when we want a changed array or accumulated data


### The Parts 
#### and simple use case

Let's say we have an array of cat names. Let's write out the skeleton of code using `#each`.

What is the `block`? 
What is the `block variable`?
What should we name the block variable?

Let's have our code simply `puts` each name. 

Can you walk through our array and explain what's happening? Take 30 seconds and tell your partner, switch.


### Using `#each`

As you're learning and hopefully realizing, return values are extemely important in Ruby. We always want to know the return value of our method. `#each` is still a method. What is the return value?

Another way to think about it, if I store the return value of my each block in a variable, what data will that variable hold?

Well what if I want to change my data? How can I save the results of the block for each element?

Example: with my array of cat names, I want to capitalize each name. How do we do this?


What to cover:

x- identify parts of our enumerable
    - block, block variable
x- Naming conventions, what should we name our block variable?

x- return vale of #each

- what do we need if we want to hold on to or save the transformation we're doing or keep track of what we're counting, etc. Basically, when we want to get something back and not just have side effects. 
    - Display with an example. If we just want to puts something, we're not really concerned with the data after we've puts-ed it, we just want the side-effect of puts-ing! For example, if I have a list of cat names, and I only want back the names that are 5 characters are shorter, how do I keep track of these if #each returns the original array?

- Quick practice to take a pulse on the class (they do)
    - given array of numbers, how can I use #each to add all these numbers together?

What questions do you have?

- If we're chuggin along:
    - What if I have a Cat class with a name attribute, exposed as a method with attr_reader. I have an array of Cat instances. How can I get each cat's name?