## Question 1
- 3 block each containing 3 floors each containing 10 rooms each containing n x n seats (n to be taken as input during runtime)
- Students should take and vacate seats while preserving the ascending order of roll numbers
- Seat is a single node containing the student as the data
	- It has intra class pointers: left, right (adjacent rows), front, back (column wise)
	- It has intra floor pointers: 