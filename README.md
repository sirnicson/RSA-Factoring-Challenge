# RSA Factoring Challenge

## Project Overview
This repository contains solutions to the RSA Factoring Challenge. The goal is to factorize given numbers into two smaller factors, which can help in breaking RSA encryption if the primes used in the encryption process are not large enough.

The challenge involves working with large natural numbers and finding their factors as quickly as possible before the target server fixes the vulnerability in their encryption.

## Requirements
Operating System: Standard Ubuntu 20.04 LTS
Programming Language: You can use any programming language of your choice
Execution Time: Each script must factorize numbers within 5 seconds
No Dependencies: The program should run without any external dependencies or installations

## Tasks

###  Task 0: Factorize all the things!
Write a program to factorize as many numbers as possible into the product of two smaller numbers. The numbers to factorize are stored in a file with one number per line.

Usage: factors <file>

<file>: A file containing natural numbers, one per line, which the program must factorize.
Input:

Each line contains a valid natural number greater than 1.
There are no empty lines or spaces before/after the numbers.
The file ends with a newline.
Output:

For each number n, print n=p*q, where p and q are factors of n.
The factors p and q do not have to be prime numbers.

```bash
Example:

bash
Copy code
6=2*3
15=3*5
143=11*13
```
Notes:
You can process the numbers in any order.
Your program will be terminated if it takes longer than 5 seconds to run.
File: factors

### Task 1: RSA Factoring Challenge
In this task, you need to factorize a number from a file. Unlike Task 0, the factors p and q must be prime numbers.

Usage: rsa <file>

<file>: A file containing a single number to factorize.
Output:

For the given number n, find its prime factors p and q such that n = p * q.
```bash
56153=233*241
```

Notes:

There is only one number in the file.
The goal is to find the prime factors as quickly as possible (under 5 seconds).
File: rsa


Historical Context
The RSA Factoring Challenge was introduced by RSA Laboratories in 1991 to stimulate research in integer factorization, a core aspect of RSA encryption. The challenge involved factoring large semiprime numbers to test the security of RSA keys. Over time, some of these numbers were factored, but many larger numbers remain unfactored today.

The challenge ended in 2007, but it served as an important benchmark for cryptography research, helping to set secure key lengths for RSA encryption.

Repository Contents
factors: A script to factorize natural numbers into two smaller numbers.
rsa: A script to factorize a number into two prime numbers.
Feel free to clone and contribute!
