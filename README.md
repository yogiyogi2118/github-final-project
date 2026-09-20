#!/bin/bash
# This script calculates simple interest given principal,
# annual rate of interest and time period in years.

# Input:
# p, principal amount
# t, time period in years
# r, annual rate of interest

# Output:
# simple interest = p * t * r / 100

echo "Enter the principal:"
read p
echo "Enter rate of interest per year:"
read r
echo "Enter time period in years:"
read t

# Using bc to handle decimal/floating-point arithmetic accurately
s=$(echo "scale=2; ($p * $t * $r) / 100" | bc)

echo "The simple interest is: $s"
