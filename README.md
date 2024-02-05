[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  1. Asymptotic analysis is concerned with the performance of an algorithm with very large inputs. In practice input sizes can vary, therefor the analysis may differ. An analysis of the time complexity at a smaller input may be drastically different from the asymptotic complexity, and smaller inputs may be what an algorithm is concerned with practically. 
  2. Asymptotic analysis is not concerened with constant factors, and in practice varying constant values can effect performance. (Memory comes to mind)
  3. Aymptotic analysis is a big picture model for algorithms, and doesn't take into account minutia such as compilers, programming language, and specific implementations. These specific implementation of an algorithm may optimize it differently, depending on the constructs of the programming language, therefor this could have an effect on the over accuracy asymptotic analysis. 

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  The asymptotic complexity of search in a binary search tree is (O)logn. log(1000) ≈ 9.965. log(10000) ≈ 13.287. These two have a ratio of approximately 1.333. If 1000 elements takes 5 seconds, then 10000 elements should take 5 * 1.333, or 6.666 seconds. 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1. The tree could be unbalanced, or even worse, already sorted (effectively creating a linked list). The search would take more time in an unbalanced tree, or worst case linear time.
  2. Hardware issues or slowdowns could be playing a role, such as a lack of the necessary amount of ram to run this algorithm efficiently, or overhead such as the operating system or other program running simultaneously. 
  3. The algorithm was implemented poorly, resulting in a slower runtime. 

Add your answers to this markdown file.
