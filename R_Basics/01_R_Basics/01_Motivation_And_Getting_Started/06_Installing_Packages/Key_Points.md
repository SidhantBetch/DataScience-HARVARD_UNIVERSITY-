# 🐦‍🔥 Note
We recommend installing packages through RStudio, rather than through R, and the code provided works in both R and RStudio. Once a package has been installed, it is technically added onto R (even if you use RStudio to install it), which is why packages must be re-installed when R is updated. However, since we use R through RStudio, any packages that are installed can be used in both R and RStudio, regardless of which one was used to install the packages.

## ⚓ Key points
- The base version of R is quite minimal, but you can supplement its functions by installing additional packages.

- We will be using tidyverse and dslabs packages for this course.

- Install packages from R console: install.packages("pkg_name")

- Install packages from RStudio interface: Tools > Install Packages (allows autocomplete)

- Once installed, we can use library(pkg_name) to load a package each time we want to use it


## 🚐 Additional Notes
- If you try to load a package with library(blahblah) and get a message like Error in library(blahblah) : there is no package called 'blahblah', it means you need to install that package first with install.packages().

- On the DataCamp interface we use for some problems in the course, you cannot install additional packages. The problems have been set up with the packages you need to solve them.

- You can add the option dependencies = TRUE, which tells R to install the other things that are necessary for the package or packages to run smoothly. Otherwise, you may need to install additional packages to unlock the full functionality of a package.

- Throughout the course materials and textbook, package names are in bold.
## 🎡 Code
```R
install.packages("dslabs")  # to install a single package
install.packages(c("tidyverse", "dslabs")） # to install two packages at the same time
installed.packages() # to see the list of all installed packages
```

## 🤦🏻 Practice: Adding Packages to R
We're going to do a quick walkthrough of how to add packages and data to R. First, we're going to see what happens if we forget to install the package first. Let's say we want to use the movielens dataset. First, open Rstudio, and try to open the movielens dataset with the following code:

```R
data(movielens)
```

We should get the following warning explaining that the dataset movielens was not found.
```R
"Warning message: In data(movielens) : data set ‘movielens’ not found"
```
This is because movielens is part of the dslabs package, which we haven't yet installed. So let's install dslabs with the following code:

```R
install.packages("dslabs")
```
However, if we try to pull the movielens data again, it still says that the dataset isn't found. That's because although we've installed dslabs, we haven't loaded it. Next, let's load it with library() using the following code:

```R
library(dslabs)
```
Now, when we try to access the movielens dataset, we will be successful.
