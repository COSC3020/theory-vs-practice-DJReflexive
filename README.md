# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1) One aspect about asymptotic analysis is that the final equation
    that shows the time complexity is often simplified from what an
    algorithm's true run time would be. For example, if an algorithms
    true run time resembles something like $\Theta(n^2 + 5n + 23)$,
    it is often simplified into the more general term of $\Theta(n^2)$.
  2) If a complexity has a loose bound, it possible that the difference
    between the loose bound and the true time complexity is so large that 
    it could be misleading to the reader.
  3) Another thing is what type of machine that algorithms are run on. Often 
    times the kind of machine that an algorithm is run on matters quite a lot. 
    For example, when running merge sort on an arduino versus running it on one 
    of the computers at the Cheyenne super computing center, the amount of time 
    it takes to execute is wildly different. Asymptotic analysis is relative
    and won't always produce exact results. It's almost like a non-exact 
    science.



- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  Binary Search Trees have an asymptotic complexity of $\Theta(logn)$ because of
  it's divide-and-conquer behavior through the tree. Since the input size of 
  1,000 results in the algorithm taking 5 seconds to execute, we can state
  mathematically that:
  
  $$c*log{_2}(1,000) = 5 seconds$$

  Solve for c:

  $$c = 5 seconds / log{_2}(1000) = 0.5017$$

  Plug back in for when n = 10000:

  $$0.5017 * log{_2}(10000) = 6.6667$$

  It will take about 6.6667 seconds to complete (or 6 and two thirds of a second) 
  to go through a tree of 10000 elements..


- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1) A possible scenerio is that the asymptotic analysis is often simplified
    to ignore constants. However, in reality, these constants do matter when
    it comes to the final run time of a program. It is simplified to give the
    reader an idea of how the algorithm *could* behave, but does not show the
    specific numbers and calculations involved.
  2) A subtle thing that might be missed when thinking about asymptotic 
    complexity is the fact that computers can only run so many processes at 
    once. It is possible other programs on the computer are halting the 
    algorithm from executing, causing a result that takes 100 seconds.
  3) Mentioned back in the first problem of this assignment  is also 
    the fact that it could be a slower machine and functions differently 
    than most. As mentioned in class, timing algorithms with timers 
    always leads to unexpected results. Asymptotic analysis is to get 
    a general idea of how fast an algorithm can run, not to provide a 
    precise formula for it.



# Sources
- None

# Plagiarism Acknowledgement

I certify that I have listed all sources used to complete this exercise, 
including the use of any Large Language Models. All of the work is my own, 
except where stated otherwise. I am aware that plagiarism carries severe 
penalties and that if plagiarism is suspected, charges may be filed against 
me without prior notice.