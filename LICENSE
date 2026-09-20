#!/bin/bash
# This script calculates simple interest given principal,
# annual rate of interest, and time period in years.

echo "Enter the principal:"
read p
echo "Enter rate of interest per year:"
read r
echo "Enter time period in years:"
read t

# Using Bash arithmetic expansion with floating-point handling via bc
s=$(echo "scale=2; ($p * $t * $r) / 100" | bc)

echo "The simple interest is: $s"
