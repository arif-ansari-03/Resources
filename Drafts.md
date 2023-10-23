#Optimizing any linear functions with finite bounds
Consider the a triangular region R bounded by x axis y axis and the line x+2y=3

If we want to optimize a function 
f(x,y) = ax+by, then the answer will lie on one of the vertices of region R. In fact this is true for any region R given that R is bounded by straight lines in xy plane

Proof: consider ax+by=c line. Now for some values of c, there’ll be some part of the line that is inside the region R. Because as we change c, we can imagine the distance of line from origin changing while remaining parallel to the line ax+by=0. So beyond some upper bound of c, there will be no part of line in R. This is the maximum value of our objective function. At this maximum point, either the line intersects only one point on R or it intersects with one of the boundaries of R. In the first case, we can say that the max lies on points of intersection of lines bounding R. In the second case, since our ax+bx=c line is coinciding with one of bounding lines of R, it is clear that it will be also passing through two of the intersection points of bounding lines. So in either case, the max lies on one of the intersection points. Similar argument is applied for minimum. This can also be extended to 3D space.


# n*n*(2^n) algorithm for maximum clique/indpendent set using bitmask dp
dp[s][i] = number of permutations of subset s, such that for every permutation ending at i there exists and edge btw every adjacent element

for (int s = 0; s < (1<<n); s++)
{
  for (int i = 0; i < n; i++)
  {
      for (int j = 0; j < n; j++)
        if (!(s&(1<<j) && edge[i][j] == 1) dp[s|(1<<j)][j] += dp[s][i]
  }
}

// now all the k - subsets such that summation of dp[s][i] (such that i is in s) is equal to k!, are cliques 
