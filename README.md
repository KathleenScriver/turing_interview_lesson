# `#each` Review
(~30 min)

## Objectives
1. Review the parts of our enumerable
1. Demonstrate using `#each` when we just want side effects
1. Practice examples using `#each` when we want a changed array or accumulated data

---
## The Parts - and simple use case

Let's say we have an array of cat names. Let's write out the skeleton of code using `#each`.

- What is the `block`? 
- What is the `block variable`?
- What should we name the block variable?

<br/>

*When do we want to use `#each`?

- Anytime we want to do something to **every** element of our array, we need to use an enumerable like `#each`.

<br/>

What do we even put inside our block though??
1. Break down the problem by focusing on a single element of the array.

    - With our array of cat names, let's just take the first element and set it equal to a variable.
`cat = "fluffy"`

2. Think about what we want to accomplish. 

    - Let's have our code simply `puts` each name of the cat name array. 

    - What do we need to do to our single `cat` to accomplish this?

<br/>

**Great!** Whatever we did to achieve this for our single element, is exactly what we want to put in our block, since our enumerator works on each element of the array, one at a time.


---
## Using `#each`

As you're learning and hopefully realizing, return values are extemely important in Ruby. We always want to know the return value of our method. 

<br/>

What is the return value of our `#each` method?

<br/>

If we just want to `puts` something, we're not really concerned with the data after we `puts` it, we just want the side-effect of `puts`

Now, what if I _do_ care about the changes I'm making in the code block though?
What if I want to change my data or accumulate my data? 

How can I save the results of the block for each element?

<br/>
<br/>



*Example: With my array of cat names, I want to capitalize each name. How do we do this?*


<br/>

*Hint:* when deciding on what your accumulator should be initialized with, think about what you want the final result to be. Do you want an array of strings? Then your accumulator should be an empty array. Do you want an array of numbers? Again, an empty array. Do you want a sum or total? What should your accumulator be initialized as?

<br/>

Can you walk through our array and explain what's happening in each iteration? Take 30 seconds and tell your partner, switch.

<br/>

*Practice*: Given my array of cat names, I only want back the cat names that are 5 characters or shorter.*

<br/>


*What questions do you have?*

<br/>

If we're chuggin along:
- What if I have a Cat class with a name attribute exposed as a method with attr_reader. I have an array of Cat instances. How can I use this array to get a transformed array with each cat's name?