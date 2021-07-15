# Operation-Research

This repository includes two projects: **OLED Lifetime** and **Graph Coloring**


* ### OLED Lifetime
  We consider an optimization problem arising in the design of controllers
for OLED displays. Our objective is to minimize the amplitude
of the electrical current flowing through the diodes which has a direct
impact on the lifetime of such a display. The optimization problem
consist of finding a decomposition of an image into sub frames with
special structural properties that allow the display driver to lower the
stress on the diodes. For monochrome images, we present an algorithm
that finds an optimal solution of this problem in quadratic time. Since
we have to find a good solution in real time, we consider an online
version of the problem in which we have to take a decision for one row
based on a constant number of rows in the look ahead. In this framework
this algorithm has a tight competitive ratio. A generalization of
this algorithm computes near optimal solutions of real-world instances
in real time. A (passive matrix) OLED display has a matrix structure
with n rows and m columns. At any crossover between a row and a
column there is a vertical diode which works as a pixel. . Consider the
contacts for the rows and columns as switches. For the time the switch
of row i and column j is closed, an electrical current flows through the
diode of pixel (𝑖, 𝑗) and it shines. Since high amplitudes of the electrical
current or high peaks of intensity respectively, are the major issues
with respect to the lifetime of the diodes we try to trade as much time
as possible for it.

  * #### Problem Definition
    Assume that we have a 3 × 3 OLED matrix, which every element of
this presents how long(number milliseconds) that diode must be on.
We represent the 3 × 3 matrix with the sum of 3 other 3 × 3 which
the first matrix close the circuit for every row for a certain amount of
time, which the total amount of time for this task(first matrix) is the
maximum value of the first matrix.
The second matrix is quite similar to the first matrix, instead of rows
every column is closed for a certain amount of time, which the total
amount of time for this task(second matrix) is the maximum value of
the second matrix.
The third matrix, for every element of the matrix a certain row and
column are closed therefore the total amount of time for this task(third
matrix) is the total sum of all the third matirx elements.


* ### Graph Coloring
  The chromatic number of a graph G is the smallest number of colors
