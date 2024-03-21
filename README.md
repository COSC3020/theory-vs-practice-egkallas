[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis is only concerned with the performance of an algorithm in terms of input size, though this is not the only factor that contributes to the algorithm's performance. Expected results from an asymptotic analysis only based on this variable will be misleading if other variables such as space complexity are not taken into account. 
  2. Big $O$ and Big $\Omega$ are not tight bounds for algorithms. Knowing this one could say that every algorithm is an element of $\Omega(1)$ and though this is by definition true, it doesn't tell us anything about the time complexity of the algorithm.
  3. If an arbitrarily large $n_0$ is chosen for the asymptotic analysis of an algorithm, the analysis is only concerned with values larger than $n_0$, therefor the behavior of all values below that is a mystery.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  The asymptotic complexity of search in a binary search tree is (O)logn. log(1000) ≈ 9.965. log(10000) ≈ 13.287. These two have a ratio of approximately 1.333. If 1000 elements takes 5 seconds, then 10000 elements should take 5 * 1.333, or 6.666 seconds. 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. The comparisons could take more time depending on the input. For example if the search involved a string comparison, which could take much longer with a larger input size, especially if a portion of that input is much larger strings. 
  2. The machines that the experiment was runned on are not made explicit, and the second run could have been on a much slower machine.
  3. The algorithm was implemented poorly, resulting in a slower runtime. 

Add your answers to this markdown file.
