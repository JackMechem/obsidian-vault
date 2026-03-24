---
created: 2026-03-24 10:43
tags:
  - class-note
---
> [!links]
> Parent: [[COMP 256 MOC]]

# Integers and Division
---
# New Notation
## Divides & Not-Divides

### Definitions
> If $a$ and $b$ are integers with $a \neq 0$, we say that $a$ divides $b$ if there is an integer $c$ such that $b = ac$.
> When $a$ divides $b$ we say that $a$ is a "factor of" $b$ and that $b$ is a "multiple of" $a$.

**Divides Operator**
$$3 | 12$$
- To specify when an integer evenly divides another integer
- Read a "3 divides 12"

**Not-divides operator**
$$3 \nmid 12$$
- To specify when an integer does *not* evenly divide another integer
- Read a "5 does not divide 12"

### Example Uses
**Determine $3 \mid 7$**
$3 \nmid 7$ because $\frac{7}{3}$ is not an integer

**Determine $3 \mid 12$**
$3 \mid 12$ because $\frac{12}{3} = 4$

### Theorem
- If $a \mid b$ and $a \mid c$, then $a \mid (b+c)$
	- Example: if $5 \mid 25$ and $5 \mid 30$, then $5 \mid (25+30)$
	 ![[Pasted image 20260324110707.png|390]]
- If $a \mid b$, then $a \mid bc$  for all integers $c$
	- Example: if $5 \mid 25$, then $5 \mid 25*c$ for all ints c
- If $a \mid b$ and $b \mid c$, then $a \mid c$

# The Division "Algorithm"
> Let $a$ be an integer and $d$ be a positive integer. Then there are unique integers $q$ and $r$, with $0 \le r \lt d$, such that $a = dq+r$ 
>
> $d$ is divisor, $a$ is dividend
> $q$ is quotient, $r$ is remainder
- We then define two operators:
	- $q = a \mid d$
	- $r = a \mod d$
## Examples
### Example 1
> What are quotient and remainder when $101$ is divided by $11$?

> [!Answer]+
> $101 = 11 \cdot 9 + 2$
> - quotient is $9$ ($2 = 101 \mid 11$)
> - remainder is $2$ ($2 = 101 \mod 11$)

### Example 2
> What are quotient and remainder when $-11$ is divides by 3?

> [!Answer]
> $-11 = 3(-4) + 1$
> - quotient is $-4$ ($-4 = -11 \mid 3$)
> - remainder is 1 ($1 = -11 \mod 3$)
>
> But $-11 = 3(-3)-2$, why not?
> - Because $r = (-2)$ does not satisfy $0 \le r \lt 3$

# Prime / Composite Numbers
- A positive integer $p$ is prime if the only positive factors of $p$ are $1$ and $p$
	- If there are any other factors, it is composite
	- Note that $1$ is *not prime or composite*, it's in its own class
- An integer $n$ is composite if and only if there exists an integer $a$ such that $a \mid n$ and $1 \lt a \lt n$

## Fundamental Theorem of Arithmetic
- Every positive integer greater than $1$ can be uniquely written as a prime or as the product of two or more primes where the prime factors are written in order of non-decreasing size

## Composite Factors
- If $n$ is a composite integer, then $n$ has a prime divisor less than or equal to the square root of $n$
- Strong inductive proof using the following logic:
- Since n is composite, it has a factor a such that $1 \lt a \lt n$
- Thus, n = ab, where a and b are positive integers greater than 1
- Either $a \le \sqrt{n}$ or $b \le \sqrt{n}$ (Otherwise, $ab \gt \sqrt{n} \cdot \sqrt{n} \gt n$)
- Thus, n has a divisor not exceeding n
- This divisor is either prime or a composite
	- If the latter, then it has a prime factor
- In either case, n has a prime factor less than n

## Showing a number is prime
> Show that $113$ is prime

> [!Answer]+
> - The only prime factors less then $\sqrt{113} = 10.63 \text{ are } 2,3,4, \text{ and } 7$
> - Neither of these divide $113$ evenly
> - Thus, by the fundamental theorem of arithmetic, $113$ must be prime

## Showing a number is composite
> Show that $899$ is prime

> [!Answer]+
> - Divide $899$ by successively larger primes (up to $\sqrt{899} = 29.98$), starting with $2$
> - We find that $29$ and $31$ divide $899$

## Primes are infinite
- Theorem (by Euclid): There are infinitely many prime numbers

- Proof my contradiction
- Assume there are a finite number of primes
- List them as follows: $p_1, p_2, ..., p_n$
- Consider the number $q = p_1 p_2 ... p_n + 1$
	- This number is not divisible by any of the listed primes
		- If we divided $p_i$ into $q$, there would result a remainder of $1$
	- We must conclude that $q$ is a prime number, not among the primes listed above.
		- This contradicts our assumption taht all primes are in the list $p_1, 0_2, ..., p_n$

# LCM, GCD
## GCD - Greatest Common Divisor
> The greatest common divisor of two integers $a$ and $b$ is the largest integer $d$ such that $d \mid a$ and $d \mid b$
> - Denoted by $\gcd(a,b)$

### Examples
- $\gcd(24,36) = 12$
- $\gcd(17,22) = 1$
- $\gcd(100,17) = 1$

### Relative Primes
- Two numbers are *relatively prime* if they don't have any common factors (other than 1)
	- Rephrased: $a$ and $b$ are relatively prime if $\gcd(25,39) = 1$
- $\gcd(25,39) = 1$ so $25$ and $39$ are relatively prime

### More on GCDs
![[Pasted image 20260324114835.png|538]]

## LCM - Least Common Multiple
- Denoted by $\operatorname{lcm}(a,b)$
- $\operatorname{lcm}(a,b) = p_1^{\max(a_1,b_1)} p_2^{\max(a_2,b_2)} ... p_n^{\max(a_n,b_n)}$
- Example: $\operatorname{lcm}(10,25) = 50$

## LCM and GCD theorem
- Let $a$ and $b$  be positive integers. Then $a \cdot b = \gcd(a,b) \cdot \operatorname{lcm}(a,b)$
![[Pasted image 20260324115549.png]]

# Pseudo-random Numbers
- Computers cannot generate truly random numbers!
- Algoriths for "random" numbers: choose 4 integers
	- Seed $x_0$: starting value
	- Modulus $m$: maximum possible value
	- Multiplier $a$: such that $2 \le a \lt m$
	- Increment $c$: between $0$ and $m$
- Formula: $x_{n+1} = (ax_n + x) \mod m$
![[Pasted image 20260324115948.png|414]]
![[Pasted image 20260324120018.png|472]]

# The Caesar Cipher
- Julius Caesar used this to encrypt messages
- A function $f$ to encrypt a letter is defined as: $f(p) = (p+3) \mod 26$
	- Where $p$ is a letter ($0$ is $A$, $1$ is $B$, $25$ is $Z$, etc...)
- Decryption: $f^{-1}(p) = (p-3) \mod 26$
- This is called a substitution cipher
	- You are substituting one letter with another.
![[Pasted image 20260324120436.png|501]]

# Rot13 encoding
![[Pasted image 20260324120509.png|499]]