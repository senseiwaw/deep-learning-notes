# Chapter 1: Applied Math and Machine Learning Basics

## 0. Key Questions
> **Goal:** Identify the mathematical foundations required for Deep Learning.

* What are the basic mathematical concepts needed to understand machine learning?
* What are the goals of machine learning?

---

## 1. Linear Algebra Prerequisites
*Focus: Concepts I don't know yet or distinct perspectives from my knowledge.*

### 1.1 Eigendecomposition of a symmetric matrix
Symmetric matrices will play a crucial role. Why ? They have a decomposition in **real eigenvalues** in a basis of **real eigenvectors**.

$$
A = Q \Lambda Q^\top
$$

Where:
* $Q$ is an **orthogonal matrix** of eigenvectors of $A$.
* $\Lambda$ is a **diagonal matrix** of eigenvalues.
* The eigenvalue $\Lambda_{i,i}$ is associated with the eigenvector in column $i$ of $Q$.

### 1.2 Singular Value Decomposition (SVD)
Unlike eigendecomposition, SVD is applicable to **any** matrix (even rectangular ones). [One of the most useful feature of SVD is that we can use it to partially generalize matrix inversion to non-square matrices](#13-the-moore-penrose-pseudoinverse)

$$
A = U D V^\top
$$

Where : 
* $A$ is an $m\times n$ matrix
* $U$ is an $m \times m$ **orthogonal matrix** and its columns contain the **left-singular vectors**
* $V$ is an $n \times n$ **orthogonal matrix** and its columns contain the **right-singular vectors** 
* $D$ is an $m \times n$ **diagonal matrix** and its columns contain the **singular values** of $A$

### 1.3 The Moore-Penrose Pseudoinverse
