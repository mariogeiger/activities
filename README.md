Input
=====

`VMIN` : array of integers of size `n`

`VMAX` : array of integers of size `n`

`WISHES` : matrix of integers of size `m x n`

where `VMIN[i] <= VMAX[i]`.
Each line of `WISHES` must contains all the integers from `0 to n-1`

Ouput
=====

`RESULT` : array of integers of size `m`

`0 <= RESULT[i] < n`

That tries to minimize the function
`sum over i of WISHES[i][RESULT[i]]^2`

The more long time the application is executed, better is the result


Example
=======

input.csv

    10,15,14
    20,16,17
    0,1,2
    2,1,0
    0,2,1
    0,1,2
    2,1,0
    0,2,1

`./activites input.csv output.csv`

output.csv

    10,15,14
    20,16,17
    0,1,2,0
    2,1,0,2
    0,2,1,0
    0,1,2,0
    2,1,0,2
    0,2,1,0