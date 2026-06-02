## 🍟 Key Points
- R was developed by statisticians and data analysts as an interactive environment for data analysis.
  
- Some of the advantages of R are that (1) it is free and open source, (2) it has the capability to save scripts, (3) there are numerous resources for learning, and (4) it is easy for developers to share software implementation.

- Expressions are evaluated in the R console when you type the expression into the console and hit Return.

- A great advantage of R over point and click analysis software is that you can save your work as scripts.

- “Base R” is what you get after you first install R. Additional components are available via packages.

## 🐦‍🔥 Code: using install.packages and library()
```R
# installing the dslabs package
install.packages("dslabs")
# loading the dslabs package into the R session
library(dslabs)
```
## 📚 Some additional notes
In RStudio, you can upload additional functions and datasets in addition to the base R functions and datasets that come with R automatically. A common way to do this is by installing packages, which often contain extra functions and datasets. For this course, there are a few packages you will need to install. You only need to install each individual package once, but after you install a package, there are other steps you have to do whenever you want to use something from that package.

To install a package, you use the code install.packages("package_name", dependencies = TRUE).

To load a package, you use the code library(package_name).

If you also want to use a dataset from a package you have loaded, then you use the code data(dataset_name). To see the dataset, you can take the additional step of View(dataset_name).
