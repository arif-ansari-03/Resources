#Optimizing any linear functions with finite bounds
Consider the a triangular region R bounded by x axis y axis and the line x+2y=3

If we want to optimize a function 
f(x,y) = ax+by, then the answer will lie on one of the vertices of region R. In fact this is true for any region R given that R is bounded by straight lines in xy plane

Proof: consider ax+by=c line. Now for some values of c, there’ll be some part of the line that is inside the region R. Because as we change c, we can imagine the distance of line from origin changing while remaining parallel to the line ax+by=0. So beyond some upper bound of c, there will be no part of line in R. This is the maximum value of our objective function. At this maximum point, either the line intersects only one point on R or it intersects with one of the boundaries of R. In the first case, we can say that the max lies on points of intersection of lines bounding R. In the second case, since our ax+bx=c line is coinciding with one of bounding lines of R, it is clear that it will be also passing through two of the intersection points of bounding lines. So in either case, the max lies on one of the intersection points. Similar argument is applied for minimum. This can also be extended to 3D space.


# n^2(2^n) algorithm for maximum clique/indpendent set using bitmask dp
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


# Fractional knapsack median method 
## Michelle Bodnar, Andrew Lohr, CLRS Solutions
First compute the value of each item, defined to be it’s worth divided by its
weight. We use a recursive approach as follows: Find the item of median value,
which can be done in linear time as shown in chapter 9. Then sum the weights
of all items whose value exceeds the median and call it M. If M exceeds W
then we know that the solution to the fractional knapsack problem lies in taking
items from among this collection. In other words, we’re now solving the fractional knapsack problem on input of size n=2. On the other hand, if the weight
doesn’t exceed W, then we must solve the fractional knapsack problem on the
input of n=2 low-value items, with maximum weight W − M. Let T(n) denote
the runtime of the algorithm. Since we can solve the problem when there is only
one item in constant time, the recursion for the runtime is T(n) = T(n=2) + cn
and T(1) = d, which gives runtime of O(n).
