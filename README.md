# Algorithms and Pseudocode

In this section, we will cover the following topics:

- Algorithms and Algorithmic Thinking
- Pseudocode

## Algorithms and Algorithmic Thinking

So, what is this thing called an algorithm? An algorithm is a series of steps to complete a task at its most basic understanding. Let's think of this in the real world for a hot minute first.

### Real-World Example of an Algorithm

The classic example of an algorithm you might have encountered in grade school is making a peanut butter and jelly sandwich.

I can remember my second-grade teacher even now. She challenged us to write out the steps to make a peanut butter and jelly sandwich.

All of us kids were excited to show off our peanut butter and jelly sandwich-making skills. We all wrote the steps to make a peanut butter and jelly sandwich.

- Get two slices of bread
- Spread peanut butter on one slice
- Spread jelly on the other slice
- Put the two slices together

Simple enough? Once my teacher started following the instructions that we kids wrote, we quickly found out we were missing steps. From forgotten knives to jelly jars that wouldn't open, we quickly learned that our instructions were not as clear as we thought.

The point of the story is not the silly mistakes we made as kids but the importance of clear and concise instructions, which is the heart of an algorithm.

Clear, concise instructions can be followed to complete a task.

### Algorithmic Thinking

Algorithmic thinking is the process of breaking down a task into a series of steps that can be followed to complete it. It is a fundamental skill in computer science and programming.

When writing an algorithm, you write instructions that a computer can follow to complete a task. This is where pseudocode comes in.

### Breaking down a Task

Let's break down a simple task: planning a vacation.

Thinking through a task can be daunting at first. Sometimes, I like to start with a notepad and pen and write a blurb about what I want to do.

For example, I might write:

```plaintext
What do I want to do?
Where do I want to go?
How much money do I have?
Where do I stay?
When do I want to go?
How do I get there?
What do I need to pack?
```

This is a good start. Even though it's a lot of questions, it's a thought process of what a vacation might look like. Also, please note that it's not in any particular order. This is okay. We can organize it.

Let's get down to business and write out the steps to plan a vacation.

```plaintext
1. Set a Budget
2. Decide on a Destination
3. Choose Travel Dates
4. Book Transportation
5. Book Accommodation
6. Plan Activities
7. Pack for the Trip
```

Remember that these steps are not set in stone. You can add or remove steps as needed. However, the overall vacation task is broken down into smaller steps that can be followed to plan a vacation.

If we wanted to start to think of this closer to code, we could:

```plaintext
set_budget = get_budget()
destination = get_destination()
travel_dates = get_travel_dates()
transportation = book_transportation(destination, travel_dates)
accommodation = book_accommodation(destination, travel_dates)
activities = plan_activities(destination)
packing_list = pack_for_trip(destination, travel_dates)
```

In this example, each task is broken down into a function that can be called to complete it. This is the essence of algorithmic thinking.

## Pseudocode

Above, we saw the beginnings of pseudocode. Pseudocode is a way to write out the steps of an algorithm in a way that is easy to understand and can be translated into code.

> Pseudocode is not just for algorithms. It can be used to plan out any task you must complete in code.

Pseudocode is written in plain English and is not tied to any particular programming language. This makes it easy to write out an algorithm's steps without worrying about syntax.

You can pseudocode in any way that makes sense to you. Here are some common ways to write pseudocode:

- Use all caps for keywords like IF, ELSE, WHILE, and FOR.
- Use indentation to show the structure of the code.

Start with your algorithmic thinking:

```plaintext
1. Input the List: Start with an unsorted list of numbers.
2. Choose a Sorting Algorithm: Decide on the sorting method. We are going to use Bubble Sort.
3. Compare Elements: Compare adjacent elements in the list.
4. Swap Elements: If the elements are out of order, swap them.
5. Repeat Until Sorted: Continue comparing and swapping until the list is sorted.
6. Output the Sorted List: Once sorted, display the result.
```

Now, let's write out the pseudocode for the Bubble Sort algorithm:

1. Input the List: Start with an unsorted list of numbers.

```plaintext
INPUT unsorted_list
```

3. Compare Elements: Compare adjacent elements in the list.

Since we have to compare each element in the list to the next element, we need to use a nested loop. The outer loop iterates over the list, and the inner loop compares the elements.

> We skipped step 2 because we use Bubble Sort as our sorting algorithm.

```plaintext
INPUT unsorted_list
FOR i FROM 0 to length(unsorted_list) - 1
    FOR j FROM 0 to length(unsorted_list) - i - 1
        IF unsorted_list[j] > unsorted_list[j + 1]
```

4. Swap Elements: If the elements are out of order, swap them.

The line `IF unsorted_list[j] > unsorted_list[j + 1]` is where we compare the elements. If the elements are out of order, we need to swap them.

```plaintext
INPUT unsorted_list
FOR i FROM 0 to length(unsorted_list) - 1
    FOR j FROM 0 to length(unsorted_list) - i - 1
        IF unsorted_list[j] > unsorted_list[j + 1]
            SWAP unsorted_list[j] and unsorted_list[j + 1]
```

5. Repeat Until Sorted: Continue comparing and swapping until the list is sorted.

The loops will continue to iterate over the list until the list is sorted.

6. Output the Sorted List: Once sorted, display the result.

We can output the sorted list outside of the loops. This way, we ensure that the list is sorted before we display the result.

```plaintext
INPUT unsorted_list
FOR i FROM 0 to length(unsorted_list) - 1
    FOR j FROM 0 to length(unsorted_list) - i - 1
        IF unsorted_list[j] > unsorted_list[j + 1]
            SWAP unsorted_list[j] and unsorted_list[j + 1]
OUTPUT sorted_list
```

## Summary

While this might seem daunting initially, breaking down a task into smaller steps is a fundamental skill in computer science and programming. It will become second nature as you practice more.

When in doubt, start with a notepad and pen and write out the steps you want to complete. This will help you think through the task and break it down into smaller steps that can be followed to complete the task.
