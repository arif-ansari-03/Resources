add a graphics section with topics like raymarching\
string stream + getline for input in c++
min max flow problems


finding num of elems greater than or equal to k in a range: 
My method. For each query we’ll calculate how many elements greater than k from 0 to r snd from 0 to l-1. Call the qr and ql. For ith query push i to L[i-1] and to R[i]. 
To calculate ql, go from left to right in A, at index i, add 1 to count of A[i] in f tree. And for each j in L[i] calc count of elem greater than the required number in the jth query

create a ds such that u can do three operations:
insert number
add given val to all elem present in the data struc
check if a number is present
