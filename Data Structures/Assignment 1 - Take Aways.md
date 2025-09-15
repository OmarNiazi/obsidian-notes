In Question 3, we were given n number of coordinates and we had to find the number of roads needed to join each coordinate to every other. The question also demanded the calculation of the number of intersection and assuming each would have 4 signals we had to return the number of signals for n coordinates as well.
The naïve approach was to use the combinations formula:

**n C r: Total n objects taking r at a time**

### Roads
For the roads we needed 2 points at a time. So putting in r = 2 simplified the formula to:
$\binom{n}{2} = \frac{n!}{2!(n-2)!} = \frac{n(n-1)}{2}$

### Signals
For the signals, we need 4 points at a time because that's the only time we gat at least 1 intersection. So the form