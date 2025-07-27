# algorithm-problems
## Chocolate 
Today is Valentine's Day. You love chocolate, so you've been waiting for this day.

The classroom has H * W seats, with H x W classmates, including you. You move from your seat and go around to your classmates' seats to get chocolate.

You're a conscientious person, so you want to give back as much as you've received.

You will be given your movement route and the number of chocolates given by your classmates sitting at each seat, so please create a program that records the number of chocolates you received in the order in which you received them.

However, you will not move to a place where there is no seat, and you will not visit the same seat more than once.

input param:
```
N H W
sy sx
s
c_{1,1} c_{1,2} ... c_{1_w}
c_{2,1} c_{2,2} ... c_{2_w}
...
c_{H,1} c_{H,2} ... c_{H_w}
```

- On the first line, you will be given N, which represents the number of trips, H, the number of seats vertically in the class, and W, the number of seats horizontally in the class, separated by a half-width space.
- On the second line, you will be given sy, which represents the row from the front where your seat is, and sx, which represents the row from the left, in that order, separated by a half-width space.
- On the third line, you will be given a string of N characters 5, which represents your travel route. The i-th character of 5 (1 <= i <= N) is "F" for moving forward, "" for moving toward, "L" for moving left, and "R" for moving right.
- The i-th row (1 <= i <= H) of the following H rows contains W integers separated by spaces. The j-th integer (1<=j<= W) on the first row, c_{i, j}, represents the number of chocolates given by the classmate sitting in the i-th column from the front and the j-th column from the left.
- There are a total of H + 3 rows of input, and a newline is inserted at the end of the last row of input values.

expected output:
Please output the number of chocolates received from classmates who sat at the seats visited, in the order they were received (in the order the seats were visited), in the following format.
```
e_1
e_2
...
e_N
```
- The expected output will consist of N lines.
- On the i-th line (1<= i <=N), output the integer e_i that represents the number of chocolates received from the classmate who sat the i-th seat visited.
- Output all integers.
- There should be a line break at the end of the last output line, and no extra characters or blank lines should be included.

condition:
```
- 1 <= N,H,W <= 100
- 1 <= sy <= H
- 1 <= sx <= W
- s is N string of "F", "B", "L", "R"
- 0 <= c_{i,j} <= 100 (1 <= i <= H, 1 <= j <= W)
- c_{sy,sx}
- dont move to the a place where there is no seat. 
- will not visit the same seat more than once.
```
For example, the case of input example 1 will look like this.
input sample:
```
3 3 3
2 1
FRB
3 6 2
0 4 1
5 0 7
```
output sample:
```
3
6
4
```
