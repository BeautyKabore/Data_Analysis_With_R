INFO 3010 - Assignment 1
================



### Q1: Compute the following values. Write code in the below chunks. (5pts)

1)  Square root of 28 (2pts)

``` r
square <- sqrt(28)
print(square)
```

    ## [1] 5.291503

3)  Round to two decimal places for pi, i.e, 3.1415926… (3pts)

``` r
round(pi,digits = 2)
```

    ## [1] 3.14

### Q2: Create the following vectors. a = (5, 10, 15, 20, 70, 120), b = (-7, 6, 18, 3, 58, -56). (10pts)

1)  create a vector ab.sum, which is add results of vector a and b
    (3pts)

``` r
vec <- c(5,10,15,20,70,120)
vec_2 <- c(-7,6,18,3,58,-56)
sum = vec + vec_2
print(sum)
```

    ## [1]  -2  16  33  23 128  64

2)  get the 3rd and 5th element of ab.sum (3pts)

``` r
print(sum[3])
```

    ## [1] 33

``` r
print(sum[5])
```

    ## [1] 128

3)  how many elements of ab.sum are greater than 30 (4pts)

### Q3: Create the following vectors with seq or rep (10pts)

1)  c(1,2,3,4,1,2,3,4) (5pts)

``` r
vec_5 <- c(seq(1,4))
rep(vec_5,2)
```

    ## [1] 1 2 3 4 1 2 3 4

1)  c(1,1,3,3,5,5,7,7) (5pts)

``` r
vec_7 = c(seq(1,7,2))
rep(vec_7, each =2)
```

    ## [1] 1 1 3 3 5 5 7 7

### Q4: Create a vector which contains 10 random integer values between -20 and +30. (5pts)

``` r
vec_8 <- c(runif(10,-20,30))
```

### Q5: Get the maximum and minumum value of a vector c(3,-5,8,12,4,2,1,7). (5pts)

``` r
vec_10 = c(3,-5,8,12,4,2,1,7)
print(min(vec_10))
```

    ## [1] -5

``` r
print(max(vec_10))
```

    ## [1] 12

### Q6: Write a R program to print the numbers from 1 to 50 and print “Fizz” for multiples of 3, print “Buzz” for multiples of 5, and print “FizzBuzz” for multiples of both. (5pts)

``` r
num <- seq(50)
for (i in num)
{
  if (i%%3==0 & i %% 5== 0)
  {
    print('FizzBuzz')
  }
  else if (i%% 5 == 0)
    {print ('Buzz')
  }
  else if (i %% 3 ==0)
  {
    print ('Fizz')
  }
  
}
```

    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "FizzBuzz"
    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "FizzBuzz"
    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "Fizz"
    ## [1] "Buzz"
    ## [1] "Fizz"
    ## [1] "FizzBuzz"
    ## [1] "Fizz"
    ## [1] "Buzz"

### Q7. Write a R program to get the unique characters of the string “This is a challenging question”. (Whitespace can be counted as a unique character) (10pts)

``` r
name <-("This is a challenging question")
as.list(strsplit(name,"")[[1]])
```

    ## [[1]]
    ## [1] "T"
    ## 
    ## [[2]]
    ## [1] "h"
    ## 
    ## [[3]]
    ## [1] "i"
    ## 
    ## [[4]]
    ## [1] "s"
    ## 
    ## [[5]]
    ## [1] " "
    ## 
    ## [[6]]
    ## [1] "i"
    ## 
    ## [[7]]
    ## [1] "s"
    ## 
    ## [[8]]
    ## [1] " "
    ## 
    ## [[9]]
    ## [1] "a"
    ## 
    ## [[10]]
    ## [1] " "
    ## 
    ## [[11]]
    ## [1] "c"
    ## 
    ## [[12]]
    ## [1] "h"
    ## 
    ## [[13]]
    ## [1] "a"
    ## 
    ## [[14]]
    ## [1] "l"
    ## 
    ## [[15]]
    ## [1] "l"
    ## 
    ## [[16]]
    ## [1] "e"
    ## 
    ## [[17]]
    ## [1] "n"
    ## 
    ## [[18]]
    ## [1] "g"
    ## 
    ## [[19]]
    ## [1] "i"
    ## 
    ## [[20]]
    ## [1] "n"
    ## 
    ## [[21]]
    ## [1] "g"
    ## 
    ## [[22]]
    ## [1] " "
    ## 
    ## [[23]]
    ## [1] "q"
    ## 
    ## [[24]]
    ## [1] "u"
    ## 
    ## [[25]]
    ## [1] "e"
    ## 
    ## [[26]]
    ## [1] "s"
    ## 
    ## [[27]]
    ## [1] "t"
    ## 
    ## [[28]]
    ## [1] "i"
    ## 
    ## [[29]]
    ## [1] "o"
    ## 
    ## [[30]]
    ## [1] "n"
