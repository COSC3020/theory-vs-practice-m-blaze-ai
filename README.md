# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

- Reasons why asymptotic analysis may be misleading:
1.) Constant factors with high performance impact are ignored by asymptotic analysis. For example, an algorithm with a higher constanct factor might perform worse than one with a lower constant factor.
2.) How data is stored and how the CPU cache works are not included in asymptotic analysis. Algorithms with better memory locality outperform those with low memor locality in practice, even if the two have equal asymptotic complexity.
3.) Asymptotic complexity assumes that the input size grows indefinitely and ignores how typical inputs are dispersed. Inputs may be significantly smaller or follow specific patterns in practice, resulting in optimizations that asymptotic analysis cannot predict.

- I would guess that finding the same element is a tree with 10,000 elements would take roughly 7 seconds. This is because the time complexity for a search operation in a binary tree is O(log n).

So, for 1,000 elements, log_2(1000) ≈ 10
and for 10,000 elements, log_2(10000) ≈ 14

you can then solve the proportion (14/10)x5 to get approximately 7 seconds.

- Why it might take 100 seconds:
  1.) The tree may not be balanced, resulting in unnecessary complexity
  2.) The recursion may not be as efficient as anticipated
  3.) External constraints such as CPU throttling or memory constraints

"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."
