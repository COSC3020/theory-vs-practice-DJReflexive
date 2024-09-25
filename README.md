# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1) One aspect about asymptotic analysis is that the final equation
    that shows the time complexity is often simplified from what an
    algorithm's true run time would be. For example, if an algorithms
    true run time resembles something like $\Theta(n^2 + 5n + 23)$,
    it is often simplified into the more general term of $\Theta(n^2)$.
  2) Ipsum...
  3) Something...



- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  Binary Search Trees have an asymptotic complexity of $\Theta(logn)$ because of
  it's divide-and-conquer behavior through the tree. Since the input size of 
  1,000 results in the algorithm taking 5 seconds to execute, we can state
  mathematically that $T(1,000) = 5 sec$. TODO!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!


- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1) One possible scenerio is that the algorithm executes a worst-case 
    situation. If the element that is being search for happens to be
    the last element to be searched in the tree, then this means the 
    algorithm has gone through every element, meaning the time complexity
    would not be $\Theta(logn)$, but instead it is $\Theta(n)$.
  2) Similarly to the first scenerio, if the elemenent being searched
    for does not appear in the tree, the same thing happens where every
    element in the tree is access, meaning the time complexity
    would not be $\Theta(logn)$, but instead it is $\Theta(n)$.
  3) Lorem...

Add your answers to this markdown file.



# Sources
- None

# Plagiarism Acknowledgement

I certify that I have listed all sources used to complete this exercise, 
including the use of any Large Language Models. All of the work is my own, 
except where stated otherwise. I am aware that plagiarism carries severe 
penalties and that if plagiarism is suspected, charges may be filed against 
me without prior notice.