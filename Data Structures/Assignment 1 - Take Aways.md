In Question 3, we were given n number of coordinates and we had to find the number of roads needed to join each coordinate to every other. The question also demanded the calculation of the number of intersection and assuming each would have 4 signals we had to return the number of signals for n coordinates as well.
The naïve approach was to use the combinations formula:

**n C r: Total n objects taking r at a time**

### Roads
For the roads we needed 2 points at a time. So putting in r = 2 simplified the formula to:

$\binom{n}{2} = \frac{n!}{2!(n-2)!} = \frac{n(n-1)}{2}$

### Signals
For the signals, we need 4 points at a time because that's the only time we gat at least 1 intersection. So the formula for that is going to be:

$\binom{n}{4} = \frac{n!}{4!(n-4)!} = \frac{n(n-1)(n-2)(n-3)}{24}$

Since each intersection has 4 signals:

$4\binom{n}{4} = 4 \cdot \frac{n(n-1)(n-2)(n-3)}{24} = \frac{n(n-1)(n-2)(n-3)}{6}$

---
But this approach is naïve for a reason and that reason is this breaks when a set of 3 or more collinear points is present.
So the next best thing is to calculate how many collinear triples are there and subtract that from the formulas above. 

For collinearity of 3 points we an use:

$\text{Area} = \frac{1}{2}\left|\det\begin{pmatrix}x_1 & y_1 & 1 \\x_2 & y_2 & 1 \\x_3 & y_3 & 1\end{pmatrix}\right| = 0$

But building this matrix would require 3 points at a time and building every possible 3 point combination is O(n<sup>3</sup>). Which is 