Finds the convex hull of a set of points
Convex hull: smallest convex set that includes given points
### Written Algorithm
Sort by x coordinates
Find points $\large P_{1}$ and $\large P_{2}$, the leftmost and rightmost points
##### Upper Hull recursively
1. find point $\large P_{max}$ (the furthest point from the line made by $\large P_{1}$ and $\large P_{2}$)
2. find upper hull of left side of $\large P_{max}$
3. find upper hull of right side of $\large P_{max}$
4. 

Use the [[Determinant]] for splitting points
