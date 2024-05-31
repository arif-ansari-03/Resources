# Competitive Programming

## Coding Platforms
[Codeforces](https://codeforces.com/)\
[SPOJ](https://www.spoj.com/)\
[HackerEarth](https://www.hackerearth.com/)\
[CodeChef](https://www.codechef.com)\
[AtCoder](https://atcoder.jp/)\
[USACO](https://usaco.guide/)\
[TopCoder Arena](https://arena.topcoder.com/index.html#/u/dashboard)\
[LeetCode](https://leetcode.com/)\
[Hackerrank](https://www.hackerrank.com/)\
[Kattis](https://open.kattis.com)\
[CSES](https://cses.fi/problemset/list/)\
[Project Euler](https://projecteuler.net)\
[CLIST](https://clist.by/)


## Useful Links
[CC - the-hyp0cr1t3](https://github.com/the-hyp0cr1t3/CC/tree/master)\
[TUTL - YouKn0wWho](https://codeforces.com/blog/entry/95106)\
[CF CP List](https://codeforces.com/blog/entry/23054)\
[Current Contests](https://clist.by/)\
[CP Algorithms](https://cp-algorithms.com/)\
[Colin Galen - Topic Streams](https://youtube.com/playlist?list=PLDjGkpToBsYCaRoQ-_S5MRxYMuKgHD62w&si=WpM6kXSUQlyB0boY)\
[List of CF Blogs 1](https://codeforces.com/blog/entry/91363)\
[List of CF Blogs 2](https://codeforces.com/blog/entry/57282)\
[List of CF Blogs 3](https://codeforces.com/blog/entry/13529)\
[Competitive Programmer's Handbook](https://usaco.guide/CPH.pdf)\
[Dynamic Programming for Computing Contests](https://dp-book.com/Dynamic_Programming.pdf#page=37)\
[Improving efficiently: beyond "just solve more problems"?](https://codeforces.com/blog/entry/66715?#comment-507869)\
[Self-deception: maybe why you're still grey after practicing every day](https://codeforces.com/blog/entry/98621)

## YouTube Channels/Links
[Errichto](https://www.youtube.com/@Errichto)

## Two Pointers, Prefix Sum, Binary Search
[Sum of all Subarrays (Prefix Sum)](https://www.geeksforgeeks.org/sum-of-all-subarrays/)/
Find smallest i in array A, such that l<=i<=r and A[i] >= k:
Maximum for subarray A[l,i] increases as i increases.
So binary search over i to find smallest i such that max of A[l,i] >= k
[Technique used here](https://codeforces.com/contest/1968/submission/263515125)

## Number Theory
[Prime Gap](https://en.wikipedia.org/wiki/Prime_gap#:~:text=The%20first%2060%20prime%20gaps,sequence%20A001223%20in%20the%20OEIS) - max prime gap upto 10^9 is 282, useful to prove some solutions\
[Linear Diophantine Equations (LDE)](https://math.libretexts.org/Courses/Mount_Royal_University/MATH_2150%3A_Higher_Arithmetic/5%3A_Diophantine_Equations/5.1%3A_Linear_Diophantine_Equations)\
[Positive solutions to LDE](https://math.stackexchange.com/questions/1470541/determining-the-existence-of-solutions-to-the-linear-diophantine-equation-ax)\
[Number of Factors](https://codeforces.com/blog/entry/22317)\
[Miller Rabin](https://en.wikipedia.org/wiki/Miller%E2%80%93Rabin_primality_test#:~:text=The%20Miller%E2%80%93Rabin%20algorithm%20can,log%20n%20of%20the%20input.)\
[Using sieve to find maximum gcd pair (Problem H)](https://codeforces.com/blog/entry/127377)

## Math
### Theorems
[Hockey Stick identity](https://mathworld.wolfram.com/ChristmasStockingTheorem.html)
### Reversible Operations
[XOR Trick](https://florian.github.io/xor-trick/)
<details>
<summary>Problems</summary>
<ul>
  <li><a href="https://codeforces.com/problemset/problem/430/C">CF 430 C</a></li>
</ul>
</details>

### Bit Manipulation
<details>
<summary>Bit by bit problems</summary>
<ul>
  <li><a href="https://codeforces.com/contest/1895/problem/D">CF 1895 D</a></li>
  <li><a href="https://codeforces.com/contest/1878/problem/G">CF 1878 G</a></li>
</ul>
</details>

## Dynamic Programming
### Bitmask DP
[Bitmasks](https://www.hackerearth.com/practice/algorithms/dynamic-programming/bit-masking/tutorial/)\
[Exponential in SOS DP is due to N-dimensional prefix sum](https://codeforces.com/blog/entry/105247)\
[Meet in the middle Bitmask](https://www.hackerrank.com/contests/countercode/challenges/subset)\
[USACO](https://usaco.guide/gold/dp-bitmasks?lang=cpp)

### Knapsack
[All possible sums using subsets using bitset, much faster in small dimensions](https://codeforces.com/contest/1970/submission/263159671)

## Graph Theory
[-is-this-fft-'s legendary blog](https://codeforces.com/blog/entry/68138)\
[Maximum Hamiltonian Path in Complete Graph](https://www.mimuw.edu.pl/~rytter/MYPAPERS/fun2012_submission_10.pdf)\
[MST minimizes the maximum weight paths](https://codeforces.com/gym/317667/problem/H)\
[Auxiliary Nodes/Graphs Example](https://codeforces.com/contest/1915/problem/G)

## Segment Trees
[AI.Cash's Efficient and Easy Segment Tree](https://codeforces.com/blog/entry/18051)\
[Merge Sort Tree](https://discuss.codechef.com/t/merge-sort-tree-tutorial/14277)

## Random blogs
[Is scanf/printf ever too slow?](https://codeforces.com/blog/entry/68043)\
[O(1) runtime prime checking](https://codeforces.com/blog/entry/79941?locale=en)

## Pitfalls
stl containers have use unsigned integers for sizes and lengths\
using bitwise shift for integers can cause issues, use long long int and use (1LL<<x) instead of (1<<x)
