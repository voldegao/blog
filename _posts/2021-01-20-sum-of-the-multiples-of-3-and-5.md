---
layout: post
title: Sum of the Multiples of 3 and 5
description: Calculate the sum of all the multiples of 3 and 5 below 1000 with javascript ... 
date: 2021-01-20 08:54:00
image: https://i.imgur.com/BD9qyC4.png
categories: [Code]
tags: [Javascript,Math]
---

In this tutorial we will calculate the sum of all the multiples of 3 and 5 below 1000. and this is a solution of the problem : 

```text
If we list all the natural numbers below 10 that are multiples of
3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.
Find the sum of all the multiples of 3 or 5 below 1000.

Source of the problem : https://projecteuler.net/problem=1
```



###### Definition:

A `multiple of n` is the product of `n` by an `integer`. In other words, a `multiple of n` is a number which, divided by `n`, gives an `integer result` , the `Euclidean division` has a `remainder` equal to `0`.

So, we will use the mod `X % N = 0` expression in order to know if the integer is a multiple of 3 or of 5

###### Solution :

So for each number x of the loop from 0 to 999, if the mod with `3 or 5` is equal to 0 then we add `x` to the `sum`.

** We used or because sometimes there are common numbers between 3 and 5 Ex: 15, 30 ...



![sum of Multiples of 3 and 5](https://i.imgur.com/BD9qyC4.png)



###### Code :

```javascript
var sum = 0
for(x = 0;x<1000;x++){
  if(x%3==0 || x%5==0){
    sum =sum +x
  }
}
console.log(sum)
```


