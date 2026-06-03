## 🐦‍🔥 Key Points

- In general, coercion is an attempt by R to be flexible with data types by guessing what was meant when an entry does not match the expected. For example, when defining x as
```
x <- c(1, "canada", 3)

```
  R coerced the data into characters. It guessed that because you put a character string in the vector, you meant the 1 and 3 to actually be character strings, "1" and "3".

- The function as.character() turns numbers into characters.

- The function as.numeric() turns characters into numbers.

- In R, missing data is assigned the value NA.
