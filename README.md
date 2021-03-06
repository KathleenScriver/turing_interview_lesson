# `#each` Review
(~30 min)

## Objectives
1. Review the parts of our enumerable

1. Demonstrate using `#each` when we just want side effects

1. Practice examples using `#each` when we want a changed array or accumulated data

<br/>
<br/>
<br/>
<br/>

---
## The Parts - and simple use case

Let's say we have an array of cat names. Let's write out the skeleton of code using `#each`.

- What is the `block`? 
- What is the `block variable`?
- What should we name the block variable?

<br/>
<br/>
<br/>
<br/>

*When do we want to use `#each`?

<br/>
<br/>


- Anytime we want to do something to **every** element of our array, we need to use an enumerable like `#each`.

<br/>

*Let's use an example. With my array of cat names, I want to `puts` each of the cat names.*

What do we even put inside our block though??
1. Break down the problem by focusing on a single element of the array.

    - With our array of cat names, let's just take the first element and set it equal to a variable.
`cat = "fluffy"`

2. Think about what we want to accomplish with this single element. In this case, how can we `puts` the cat's name?  *Think about this to yourself for 10 seconds.*


<br/>

**Great!** Whatever we did to achieve this for our single element, is exactly what we want to put in our block, since our enumerator works on each element of the array, one at a time.

So what would our final code look like to accomplish our goal of `puts` each cat's name?

<br/>
<br/>

*Practice:* I want to puts the length of each cat's name.

<br/>



---
## Using `#each`

As you're learning and hopefully realizing, return values are extemely important in Ruby. We always want to know the return value of our method. 

<br/>

What is the return value of our `#each` method? *Think to yourself for a few seconds.*

<br/>

If we just want to `puts` something, we're not really concerned with the data after we `puts` it, we just want the side-effect of `puts`.

<br/>


Now, what if I _do_ care about the changes I'm making in the code block though?
What if I want to change my data or accumulate my data? 

How can I save the results of the block for each element?

<br/>


*Example: With my array of cat names, I want to capitalize each name. How do we do this?*


<br/>

*Hint:* when deciding on what your accumulator should be initialized with, think about what you want the final result to be. Do you want an array of strings? Then your accumulator should be an empty array. Do you want an array of numbers? Again, an empty array. Do you want a sum or total? What should your accumulator be initialized as?

<br/>

Breakout Rooms to practice! Remember to break down the problem for a single element and think about your accumulator (if needed). (5 min)

<br/>

*Practice*: Given my array of cat names, I only want back the cat names that are 5 characters or shorter.

<br/>

*Practice:* Given my array of cat names, I want to find the total number of characters of all the cat names.

<br/>

**What questions do you have?**

<br/>

If we're chuggin along:
- What if I have a Cat class with a name attribute exposed as a method with attr_reader. I have an array of Cat instances. How can I use this array to get a transformed array with each cat's name?