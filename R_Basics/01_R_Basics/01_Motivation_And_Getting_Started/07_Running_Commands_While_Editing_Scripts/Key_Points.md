# 🍟 Note
The code in this video contains a pipe (i.e. %>%) and the ggplot() function. Pipes are from the tidyverse package and are covered in a later section of the course, but ggplot() is not covered in R Basics. You do not need to be able to be able to use pipes or ggplot() at this point.

## 📚 Key points
- RStudio has many useful features as an R editor, including the ability to test code easily as we write scripts and several autocomplete features.

- Keyboard shortcuts:

  - Save a script: Ctrl+S on Windows and Command+S on Mac

  - Run an entire script:  Ctrl+Shift+Enter on Windows Command+Shift+Return on Mac, or click "Source" on the editor pane

  - Run a single line of script: Ctrl+Enter on Windows and Command+Return on Mac while the cursor is pointing to that line, or select the chunk and click "run"

  - Open a new script: Ctrl+Shift+N on Windows and Command+Shift+N on Mac
  
# 🐦‍🔥 Code
```R
library(tidyverse)
library(dslabs)
data(murders)

murders %>%
    ggplot(aes(population, total, label=abb, color=region)) +
    geom_label()
```
