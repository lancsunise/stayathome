---
title: "Stay at Home Activities"
subtitle: "Version 1"
author: [SCC UG Wellbeing & Experience, Lancaster University]
date: "May 2020"
subject: "Markdown"
keywords: [Markdown, Example]
book: true
classoption: [oneside]
titlepage: true
titlepage-rule-color: "360049"
titlepage-background: "template/background.pdf"
toc: true
toc-own-page: true
toc-title: Index
colorlinks: true
...

# Why This Booklet?

The core reason is the disturbance caused by the unfortunate coronavirus. As the virus caused cancelling of exams, we hoped that the time you would use to prepare for exams could be used somewhere else. This booklet is a compilation of some interesting computer science (CS) challenges, readings and facts. It's meant to be informative and give you some directions for fullfiling your free time for the rest of this term. Through some CS challenges, the aim of this booklet is to also engage you to be active on a dedicated Moodle forum. The dedicated forum is available in the general discussion section for your respective year (e.g. UG Second Year 19/20). Feel free to join in and discuss any parts of this booklet. Or even better, feel free to share any interesting (CS) challenges, news, facts, interesting ideas, etc. that you came across and think are worth mentioning or solving.

This booklet is prepared for all undergraduate students. So, you may come across something you haven't learnt yet. No worries, if you are interested enough you can search for keywords mentioned in this document. On the other hand, if you are a final year student you may find some parts easy. In this case, follow the references in this document to learn some new skills. At the end of the day, everyone should hopefully find some useful references/ideas to keep themselves busy during the rest of this term.

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

# Useful Readings

This chapter contains a collection of books and tutorials. They are divided in several topics. They are mostly a subset of books and tutorials that I am aware of. Computer Science is a wide area however, so consider contributing some of your favourite CS books/tutorials here. Read the chapter "Participation" to see how to contribute. Please note that some books will be available in the University's online library, whilst some won't. Where possible, books which are freely available are favoured.

## Programming Languages

Once you've learnt variables, if statements, loops and functions you can code pretty much anything you want. So, should you stop acquiring any extra programming knowledge? No. There is so much more with virtually any language to learn about. C++ has a reputation to be one of the most complicated languages out there. Why? Because the language is so rich in different concepts that there is almost always something new to learn. Java, C#, etc. are also rich languages so I'm almost certain that once you open one of the books below you will find something you didn't know. Without further ado, below are some books that may be useful to extend your knowledge.

### Java

+ Java: The Complete Reference by Herbert Schildt: as the title says, this book provides a detailed reference of all Java features. You should probably use this book to find relevant topics of your interest, rather than reading the whole book in one go.
+ Thinking in Java by Bruce Eckel: relatively famous book on Java, similar to the one above, but needs a new version. It's here mostly as a reference (though, don't make me stop you to have a look at it, writing is really good!)
+ Effective Java by Joshua Bloch: this is a more advanced book suggesting some good practices to consider when coding in Java.

### C/C++

+ The C Programming Language by Brian Kernighan and Dennis Ritchie: in my opinion this is one of the most important programming books. It shows how things in computer science are not actually moving that quick. Yes, we can new things, but the main concepts remain.
+ C++ Primer by Josee Lajoie and Stanley B. Lippman: this book is virtually a reference book as well. It contains most of the modern C++ features and it is a pretty decent book to have in your collection if you're into C++.

### Other Languages

> Everyone has their favourite languages. If your favourite language isn't covered here, which book or tutorial did you follow to learn the language. Fancy sharing that with your peers? Jump to "Participation" to see how to contribute.

## Concurrency

+ Java Concurrency in Practice by Brian Goetz et al.: this is a Java oriented book, but describes concurrency related concepts which be applied across different languages
+ [Java Concurrency and Multithreading Tutorial](http://tutorials.jenkov.com/java-concurrency/index.html): very detailed tutorial on concurrency in Java if you want to avoid a book.

## Object Oriented Programming

+ Design Patterns: Elements of Reusable Object-Oriented Software by Gamma et al.: this book is a classic. Have you heard the phrase "Gang of Four"? Well, this is the book from the gang in question. Four authors who influenced OOP from the 90s onwards.
+ [Game Programming Patterns by Bob Nystrom](https://gameprogrammingpatterns.com/): in my opinion the best book to explain desing patterns in an interesting way + using many game examples. Very useful if you're on an SCC.210 module. The best of all, the online version is free. Also, each pattern is more or less self-contained so read only what you're interested in.

## General Software Engineering

+ Code Complete by Steve McConnell: a great book to learn how to improve your coding skills!
+ The Pragmatic Programmer by Hunt and Thomas: book which very well complements Code Complete. This book is another classic amongst software people.
+ Clean Code by Robert C. Martin: another great book that teaches you how to write good code - spoiler alert it has to do a lot with avoiding variable names such as l, m, z... So how to call variables, functions etc.? This is the book to look at.
+ Clean Architecture by Robert C. Martin: once you can write clean code, you need to know how to structure it well. This book is a really good read for those who want to be software professionals.
+ Agile Estimating and Planning, by Mike Cohn: how do agile teams work? What is team's velocity? How to estimate the size of tasks? This book is a really good guide to understand agile development.
+ [Docker](https://docs.docker.com/get-started/overview/): learn how modern applications are deployed nowadays.
+ [Jenkins Blue Ocean (Continous Integration)](https://www.jenkins.io/projects/blueocean/): have a look at how companies manage their software lifecycle.
+ [Git workflow - trunk based development](https://trunkbaseddevelopment.com/): a super useful tutorial on how to use version control systems effeciently

## Cryptography

+ Cryptography Engineering: Design Principles and Practical Applications by Ferguson et al.: this book is probably a good start if you're interested in the field. It's comprehensive but still not too complicated.

## Data Science

+ Foundamentals of Data Visualisation by Claus O. Wilke: next time you generate graphs from your user study for SCC.210 (yes, again SCC.210, but also useful everywhere else where you need to present some graphs), first have a look at this book. This book will tell you precisely how to make graphs so that during the Q&A time you don't get a question what values are on the $x$-axis. This book is truly great and you can read it for free online!
+ Data Science from Scratch - First Principles with Python: many books teach concepts and then they apply those concepts using some existing solutions. This book is different. It goes through most concepts from scratch - i.e. by implementing some basic operations such as variance, covariance, correlation, etc. An interesting read for sure.

## Machine Learning

+ Data Mining: Practical Machine Learning Tools and Techniques by Hall et al.: there are too many books on machine learning that it's difficult to choose which to list. This book is from University of Waikato academics who also created a tool called Weka (try to guess where Waikato is...). Anyhow, I believe this book gives a good foundation for machine learning and you can also practice your knowledge in Weka (which requires no coding).
+ Foundations of Machine Learning by Mohri et al.: the big benefit of this book is that it's free! It also covers very many machine learning concepts. You should totally try it.
+ [Kaggle](https://www.kaggle.com/competitions): famous platform for machine learning competitions. There is one very relevant challenge going on there, which is the call for [help to better understand Covid-19](https://www.kaggle.com/covid19).

## Graphics

+ [Learn OpenGL](https://learnopengl.com/): this tutorial should give you a head start into computer graphics. There is also an offline PDF version of the tutorials freely available.
+ [Start making a 2D game](https://lazyfoo.net/tutorials/SDL/): alternative: [libgdx (Java)](https://github.com/libgdx/libgdx/wiki)
+ [Start making a 3D game](https://learn.unity.com/tutorials): alternative: [jMonkeyEngine (Java)](https://jmonkeyengine.org/docs/), [Unreal Engine (C++)](https://docs.unrealengine.com/en-US/SiteIndex/index.html?versions=4_9)

## Biographies

+ Founders at Work by Jessica Livingston: OK, perhaps not a biography in a traditional sense of the word, but if you're interested on how many software companies started (e.g. Yahoo, Flickr, TripAdvisor) this book is for you. It contains a collection of interviews with founders of many software companies.


# Interesting CS Facts

1. Linus Torvalds developed the first version of Linux when he was roughly your age. Read his [first email](https://groups.google.com/forum/#!msg/comp.os.minix/dlNtH7RRrGA/SwRavCzVE7gJ) where he announced Linux.

2. We don't hear often about Claude Shannon, but his [article](https://web.archive.org/web/19980715013250/http://cm.bell-labs.com/cm/ms/what/shannonday/shannon1948.pdf) is the founding work of the field of information theory. Maybe you've heard about the _information entropy_ - that's from Shannon's work. One very useful application of the information entropy is loseless compression.

3. The term "software engineering" was coined by Margaret Hamilton, who is one of the first computer programmers. She was director of the software engineering at MIT which developed on-board flight software for [NASA's Apollo program](https://en.wikipedia.org/wiki/Margaret_Hamilton_(software_engineer)).

4. HP, Microsoft and Apple have one very interesting thing in common – they were all started in a garage.

5. This one is a bit controversial (so perhaps not a fact). Object oriented (OO) languages are all about the four primary features: encapsulation, abstraction, inheritance and polymorphism. But are they really? See what [Uncle Bob](https://youtu.be/QHnLmvDxGTY?t=2059) thinks about OO.

6. It is estimated that Google consumes the energy of [200,000 households](https://business.directenergy.com/blog/2017/november/powering-a-google-search) each year. And all this in order to index less than 1% of the information available on the Internet.

7. Only [8%](https://money.howstuffworks.com/currency.htm) of the world's currency is physical money, the rest is on computers.

8. The video game industry [has sales greater](https://www.econotimes.com/The-Gaming-Industry-Is-Now-Bigger-Than-Hollywood-1558784) than Hollywood box office sales.

9. [Add some interesting fact that you know here](https://github.com/lancsunise/stayathome)

# Participation

## Spotted an error?

Have you found any errors somewhere in the text? Or you want to contribute some challenges, cool URLs, or other CS facts. Consider contributing.

## How can I contribute?

The way (some) software professionals do. Via pull requests on github. This booklet is shared [here](https://github.com/lancsunise/stayathome).

When developers work on a big project they use a version control system (e.g. git). Keeping code under a version control helps immensely to build software. But, a version control is not only limited to the code. Text, books, or virtually any files are allowed under a version control system, allowing you to see the whole history of files. The benefit of a version control system in our case is that if you find an error in the text, then you have the complete freedom to directly patch the error and create a pull request. If your correction is correct, I will merge the changes into the master branch.

## Branches

The copy of this booklet lives on the master branch. To make changes, you need:

1. Clone the repository locally on your computer:
```
git clone https://github.com/lancsunise/stayathome
```
2. Create a new branch where you will apply a fix (you can replace my_fix_branch with any other name describing what you are fixing):
```
git checkout -b my_fix_branch
```
3. Apply the fix

## Pull Requests

...

# References

