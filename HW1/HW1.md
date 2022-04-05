HW 1
================

### Question 3

#### 3.1

``` r
# Set seed so my answers won't change when I knit this

set.seed(5645)

# Draw random variables

vars <- rnorm(10, 5, 5)
```

#### 3.2

``` r
# Get the mean of vars

mean(vars)
```

    ## [1] 7.606588

The mean of my 10 random variables is significantly higher than the true
mean. It is 2.5 bigger than the true mean of 10.

#### 3.3

``` r
# Calculate SE

sdev <- sd(vars)

serror <- sdev / sqrt(10); serror
```

    ## [1] 1.792275

The standard error is 1.8.

#### 3.4

``` r
# Set seed again because its not staying the same

set.seed(5645)

# Run the same thing 1000 times

means <- sapply(1:1000, function(x){
  mean(rnorm(10,5,5))
}) 

hist(means)
```

![](HW1_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

#### 3.5

``` r
# Get standard deviation 

sd(means)
```

    ## [1] 1.547885

The standard deviation is 1.5.

#### 3.6

The standard is smaller than it is in part 3. This is expected because
as we run the simulation more times, the outcomes should be less noisy,
which corresponds to a smaller standard error.