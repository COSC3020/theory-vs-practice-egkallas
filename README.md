[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis is only concerned with the performance of an algorithm in terms of input size, though this is not the only factor that contributes to the algorithm's performance. Expected results from an asymptotic analysis only based on this variable will be misleading if other variables such as space complexity are not taken into account. 
  2. Big $O$ and Big $/Omega$ are not tight bounds for algorithms. Knowing this one could say that every algorithm is an element of $/Omega(1)$ and though this is by defition true, it doesn't tell us anything about the time complexity of the algorithm.
  3. Aymptotic analysis is a model for the bounded growth rate of algorithms, and doesn't take into account minutia such as compilers, programming language, and specific implementations. The asymptotic complexity of an algorithm does not change based on these factors, but these factors can effect the overall runtime for the algorithm. The asymptotic complexity only gives a universal growth rate for the algorithm, and the actual runtime can vary. Additionally, the asymptotic complexity of an algorithm doesn't change based on implementation if the constant factors and dominating term remain the same. 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  The asymptotic complexity of search in a binary search tree is (O)logn. log(1000) ≈ 9.965. log(10000) ≈ 13.287. These two have a ratio of approximately 1.333. If 1000 elements takes 5 seconds, then 10000 elements should take 5 * 1.333, or 6.666 seconds. 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. The tree could be unbalanced, or even worse, already sorted (effectively creating a linked list). The search would take more time in an unbalanced tree, or worst case linear time.
  2. Hardware issues or slowdowns could be playing a role. With a larger input, more hardware resources could be being used than a smaller input. If there are temporary variables being used each time the find is called recursively, these can add up and negatively effect the space complexity, thus slowing down the processing. 
  3. The algorithm was implemented poorly, resulting in a slower runtime. 

Add your answers to this markdown file.
