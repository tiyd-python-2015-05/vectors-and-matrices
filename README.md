# Matrix Math

## Description

Implement various matrix math functions using no math libraries.

## Objectives

### Learning Objectives

After completing this assignment, you should understand:

* 2 Dimensional List traversal
* Introductory Linear Algebra concepts

### Performance Objectives

After completing this assignment, you should be able to:

* Perform mathematical operations on complex list structures

## Details

### Deliverables

* A Git repo called matrix-math containing at least:
  * `README.md` file explaining how to run your project
  * a module called `matrix-math`
  * tests for `matrix-math`

### Requirements

* Passing unit tests
* No PEP8 or Pyflakes warnings or errors
* No use of math libraries - only built in `+ - / *` operators

## Normal Mode

Implement these Linear Algebra functions:

Matrix Addition:

*Shape Rule: Dimensions of each matrix must be the same.*

```
[[a b]   +  [[w x]   =   [[a+w b+x]
 [c d]]      [y z]]       [c+y d+z]]

Matrix + Matrix = Matrix
```

Matrix-Scalar Multiplication:

*Shape Rule: None*

```
[[a b]   *  Z   =   [[a*Z b*Z]
 [c d]]              [c*Z d*Z]]

Matrix * Scalar = Matrix
```

Matrix-Vector Multiplication:

*Shape Rule: The number of rows of the vector must equal the number of columns of the matrix.*

```
[[a b]   *  [x   =   [a*x+b*y
 [c d]       y]       c*x+d*y
 [e f]                e*x+f*y]

Matrix * Vector = Vector
```

Matrix-Matrix Multiplication:

*Shape Rule: The number of columns of the first matrix must equal the number of rows of the second matrix.*

```
[[a b]   *  [[w x]   =   [[a*w+b*y a*x+b*z]
 [c d]       [y z]]       [c*w+d*y c*x+d*z]
 [e f]                    [e*w+f*y e*x+f*z]]

Matrix * Matrix = Matrix
```

* Create asserts that ensure that the function returns a correctly calculated data structure
* Create each function according to the above specifications
* Each function should check the shape of the incoming matrix/vector before any calculations
* Refactor as much reusable code as possible

## Hard Mode

In addition to the requirements from **Normal Mode**:

* Implement the above functions without using any `for` loops

## Notes


## Reading

[Linear Algebra Review and Reference](http://cs229.stanford.edu/section/cs229-linalg.pdf)

[Traversing a two-dimensional "array"](https://mail.python.org/pipermail/tutor/2008-June/062425.html)
