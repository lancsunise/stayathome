# Coding Challenges

## Introduction

This chapter contains a few code challenges reused from \texttt{LeetCode}. If you haven't heard of \texttt{LeetCode}, it's an online programming learning platform that contains 1000+ different coding chanllenges ranging from easy to hard. \texttt{LeetCode} is not the only such platform. Similar platforms are \texttt{HackerRank}, \texttt{TopCoder}, \texttt{geeksforgeeks}, \texttt{CodeChef} and probably many many more. What are these platforms used for? Mostly for preparing for coding interviews with software companies. Have a look at [InterviewInsider](https://interviewinsider.io/) at types of questions asked in interviews across different large software companies. For most of them you will see that companies look for medium difficulty questions (as classified by \texttt{LeetCode}).

This chapter suggests several interesting easy and medium difficulty questions, but if you find it too difficult or too easy, feel free to hone into other \texttt{LeetCode} questions. To make things a bit more interesting, we suggest that you discuss these challenges with your peers via Moodle discussion ([Year 1](), [Year 2](), [Year 3]()). Feel free to share ideas, hints, time and space complexity of your solutions. If you are struggling to find a solution (and \texttt{LeetCode} doesn't provide one), ask your peers for help. Start new discussions for questions that are not in this booklet. The aim is to stay engaged and have fun in this "no exam preparation" period. The only things we ask is to be polite and not share complete code solutions, as then the fun stops.

## Big O

Before starting any coding, here is one warm up challenge.

> Challenge 0: Let's say you have a file on a hard drive you want to send to your friend. Your friend needs to get the file as fast as possible. How should you send it? [@CtCI]

If you haven't come across the term in the title yet don't worry. Hint: descriptive solutions are good enough! Also, don't forget to use the Moodle forum to discuss your solution(s) for this challenge (unless if you have come across this challenge before, in which case feel free to provide hints to your peers but no full answers).


## Know your algorithms and data structures

Most of you have come across algorithms and data structures even if you haven't always formally called them this way. Let's test this. Have you used arrays before? Sure you have. So now you know how to place values one after another into the memory for an efficient way to access them. Have you used ArrayList? It's another structure, very similar to the vanilla arrays, with some extra neat features. In any case, now is a good time to search the Internet and find more about algorithms and data structures. They will be immenisley useful for the challenges below and beyond. Consider the next challenge as a good **start** for testing (or starting to acquire) your knowledge about algorithms and data structures:

> Challenge 0.1: Between ArrayList and LinkedList (Java), which one is faster? In what cases is one faster than the other? What's the time and space complexity of each for different operations (e.g. add, remove, etc.)?

Below is a table of core data structures, algorithms and concepts [@CtCI]. Use this summer to explore them.

------------------------------------------------------------------
Data structures         Algorithms              Concepts
----------------------  --------------------    ------------
Linked Lists            Breadth-First Search    Bit Manipulation

Trees, Tries & Graphs   Depth-First Search      Memory (heap vs. stack)

Stacks & Queues         Binary Search           Recursion

Heaps                   Merge Sort              Dynamic Programming

Vectors/ArrayLists      Quick Sort              Big O Time & Space

HashTables
------------------------------------------------------------------

> Hint: if you are a final year student, start brushing up on these concepts (of course, if you want to get into development...)

OK, now you are good to go to some coding challenges.

## Two Sum

> Difficulty: easy; Link: [LeetCode](https://leetcode.com/problems/two-sum/)

Given an array of integers, return indices of the two numbers such that they add up to a specific target. You may assume that each input would have exactly one solution, and you may not use the same element twice. Example:

> ```
> Given nums = [2, 7, 11, 15], target = 9,
> Because nums[0] + nums[1] = 2 + 7 = 9,
> return [0, 1].
> ```

This is another challenge for warming up yourself. Of course, there are many possible solutions to this exercise, but some solutions are better than others. One advice is to start with the simplest solution and then improve. Try not to look at the solution tab on \texttt{LeetCode} before you try really hard to come up with a solution yourself.

An obvious solution to this exercise would be a brute force approach (using two loops). That would work, though ineffeciently on big arrays. More precisely, the brute force approach would cost us $O(n^2)$ in time complexity and $O(1)$ in space complexity. Apart from the brute force solution, \texttt{LeetCode} offers two more possible solutions. Both other solutions with time complexity of $O(n)$ and space complexity $O(n)$. Before you look at these, try to see how you would bring the time and space complexity down to $O(n)$.

> Challenge 1: Can this problem be done even more effeciently? Let's say, time complexity $O(n)$ and space complexity $O(1)$. Forum discussion is more than welcome here!

## Subsets

> Difficulty: medium; Link: [LeetCode](https://leetcode.com/problems/subsets/)

Given a set of **distinct** integers, nums, return all possible subsets (the power set).
Note: The solution set must not contain duplicate subsets.

Example:

> Input: nums = [1,2,3]

> Output:
> ```[
  [3],
  [1],
  [2],
  [1,2,3],
  [1,3],
  [2,3],
  [1,2],
  []
 ]```

> Challenge 2: Find a solution which doesn't exceed time and space complexity of $O(n x 2^n)$.
 
## Container With Most Water

> Difficulty: medium; Link: [LeetCode](https://leetcode.com/problems/container-with-most-water/)

Given n non-negative integers $a_1$, $a_2$, ..., $a_n$ , where each represents a point at coordinate ($i$, $a_i$). n vertical lines are drawn such that the two endpoints of line $i$ is at ($i$, $a_i$) and ($i$, $0$). Find two lines, which together with x-axis forms a container, such that the container contains the most water.

> Challenge 3: Can you find an $O(n)$ time complexity and $O(1)$ space complexity solution?

## More Challenges

This is just a small subset of challenges. Let's say for one week of fun. You can find many more on the websites provided in the Introduction and work on them at your own pace. P.s. If you come across interesting ones, share them on Moodle. If you've had enough of this type of exercises, then perhaps you find some interesting readings in the next chapter. 
