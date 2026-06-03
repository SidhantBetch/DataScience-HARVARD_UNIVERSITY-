# 🐦‍🔥 Correction
At 3:54 in the video, the output for min(murders$total) should read: 2.


## ⚓ Key Points

- The function sort() sorts a vector in increasing order.

- The function order() produces the indices needed to obtain the sorted vector, e.g. a result of  2 3 1 5 4 means the sorted vector will be produced by listing the 2nd, 3rd, 1st, 5th, and then 4th item of the original vector.

- The function rank() gives us the ranks of the items in the original vector.

- The function max() returns the largest value, while which.max() returns the index of the largest value. The functions min() and which.min() work similarly for minimum values.


## 🚐 Code
```R
library(dslabs)
data(murders)
sort(murders$total)

x <- c(31, 4, 15, 92, 65)
x
sort(x)    # puts elements in order

index <- order(x)    # returns index that will put x in order
x[index]    # rearranging by this index puts elements in order
order(x)

murders$state[1:10]
murders$abb[1:10]

index <- order(murders$total)
murders$abb[index]    # order abbreviations by total murders

max(murders$total)    # highest number of total murders
i_max <- which.max(murders$total)    # index with highest number of murders
murders$state[i_max]    # state name with highest number of total murders

x <- c(31, 4, 15, 92, 65)
x
rank(x)    # returns ranks (smallest to largest)

```
