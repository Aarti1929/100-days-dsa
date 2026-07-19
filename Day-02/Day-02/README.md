# Day 02 - Greatest Common Divisor (GCD)

## Problem
Find the Greatest Common Divisor (GCD) of two integers.

## Algorithm
- Read two integers.
- Apply the Euclidean Algorithm:
  - gcd(a, b) = gcd(b, a % b)
- Repeat until `b == 0`.
- Print `a`.

## Time Complexity
O(log(min(a, b)))

## Space Complexity
O(1)

## Language
C++
