---
created: 2026-03-23 13:30
tags:
  - class-note
---
> [!links]
> Parent: [[COMP 256 MOC]]

# Info
- Thursday, March 26th
- Held on canvas

# Topics
- Sets
- Sequences (sums/loops)
- Proofs
- Counting

# Previous Quiz Questions

## Quiz 1

### Question 1
$$\text{If } |A| = 4, \text {what is } |P(P(A))|$$
- $2^{16}$
- $16$
- $32$
- $2^4$

> [!Answer]-
> $2^{16}$
> 
> Explanation: 
> The number of elements in a power set is always $2^{|S|}$. 
> $|P(A)| = 2^{4} \implies |P(P(A))| = 2^{2^4} = 2^{16}$
### Question 2
$$\text{Which statements are always true for set} A? \text{ (select all correct)}$$
- $\emptyset \subseteq a$
- $\emptyset \subset A$
- $A  \subseteq \emptyset$
- $A \subseteq A$
- $A \subset A$

> [!Answer]-
> - $\emptyset \subseteq a$
> - $A \subseteq A$
> 
> Explanation:
>   1. By definition, the empty set $\emptyset$ is a subset of every set.
>   2. Every set is a subset of itself
### Question 3
$$\text {Which sets have exactly 2 elements? (select all correct)}$$
- $\{\{1,2\}\}$
- $\{ \emptyset , \{ \emptyset \}\}$
- $\{\{\emptyset\}\}$
- $\{1,2\}$
- $\{\{1\},\{2\}\}$

> [!Answer]-
> - $\{ \emptyset , \{ \emptyset \}\}$
> - $\{1,2\}$
> - $\{\{1\},\{2\}\}$
> 
> Explanation:
> 	Look at the curly-braces and figure it out
### Question 4
$$\text {Which of the following is true? (select all correct)}$$
- $\emptyset \times A = A$
- $A \times B = B \times A$
- $A \times \emptyset = \emptyset$
- $|A \times B| = |B \times A|$

> [!Answer]-
> - $A \times \emptyset = \emptyset$
> 	- You are essentially multiplying A with zero, so you get an empty set.
> - $|A \times B| = |B \times A|$
> 	- Since you are comparing cardinality (size) the order of the elements in the pairs doesn't matter; therefore they are equal.
### Question 5
$$\text {Which statements are always true? (select all correct)}$$
- $|P(A)| = |A|$
- $|P(A)| = 2^{|A|}$
- $|P(A)| = |A|^2$
- $|P(A)| = 2|A|$

> [!Answer]-
> - $|P(A)| = 2^{|A|}$
> 	- Asking for the formula for the cardinality of a power set, formula used in [[#Question 1]]
### Question 6
$$\text{If } |A| = |B| \text{, what is true? (Select all correct answers)}$$
- $A \cap B \neq \emptyset$
- $|A \cup B| = |A|$
- $\text{none}$
- $|A \cap B| = |A|$
- $A = B$

> [!Answer]-
> $\text{none}$
### Question 7
$$\text{If } A = \emptyset \text{, what is true? (Select all that are correct)}$$
- $\emptyset \in A$
- $\emptyset \subseteq A$
- $|A| = 1$
- $A \subset \emptyset$

> [!Answer]-
> - $\emptyset \subseteq A$
### Question 8
$$\text{Which of the following are elements of } P(\{1, 2\})\text{? (Select all that are correct)}$$
- $\emptyset$
- $\{1, 2\}$
- $1$
- $\{2\}$
- $\{1\}$

> [!Answer]-
> - $\emptyset$
> - $\{1, 2\}$
> - $\{2\}$
> - $\{1\}$
### Question 9
$$\text{If } A=\{a, b, c\}, \text{ how many elements does } P(A) \text{ have?}$$
- $9$
- $8$
- $3$
- $6$

> [!Answer]-
> - $8$
### Question 10
$$\text{Which are always subsets of } A \cup B \text{? (Select all correct answers)}$$
- $B - A$
- $A - B$
- $A \cap B$
- $A$
- $B$

> [!Answer]-
> - $B - A$
> - $A - B$
> - $A \cap B$
> - $A$
> - $B$
### Question 11
$$\text{Which expressions describe the same region? (Select all correct answers)}$$
- $A - (A \cap B)$
- $A \cap B$
- $A - B$
- $A \cap B^C$

> [!Answer]-
> - $A - (A \cap B)$
> - $A - B$
> - $A \cap B^C$
### Question 12
$$\text{If } A \subset B, \text{ which must be true? (Select all that are correct)}$$
- $A \subseteq B$
- $A \neq B$
- $|A| < |B|$
- $B \subseteq A$

> [!Answer]-
> - $A \subseteq B$
> - $A \neq B$
> - $|A| < |B|$
### Question 13
$$\text{Let } A=\{1, 2, 3, 4\} \text{ and } B=\{3, 4, 5\}. \text{ What is } A - B?$$
- $\{1, 2\}$
- $\{3, 4\}$
- $\{1, 2, 5\}$
- $\{3, 5\}$
- $\{5\}$

> [!Answer]-
> - $\{1, 2\}$
### Question 14
$$\text{Which are true for all sets?}$$
- $\emptyset - A = \emptyset$
- $A \cap \emptyset = \emptyset$
- $A \cup \emptyset = A$
- $A - \emptyset = \emptyset$

> [!Answer]-
> - $\emptyset - A = \emptyset$
> - $A \cap \emptyset = \emptyset$
> - $A \cup \emptyset = A$
### Question 15
$$\text{Which situation is impossible? (Select all that are correct)}$$
- $|A| = 8, |B| = 8, |A \cap B| = 0$
- $|A| = 5, |B| = 7, |A \cap B| = 3$
- $|A| = 6, |B| = 6, |A \cap B| = 6$
- $|A| = 10, |B| = 12, |A \cap B| = 15$

> [!Answer]-
> - $|A| = 10, |B| = 12, |A \cap B| = 15$
### Question 16
$$\text{Evaluate } |P(C)| \cdot |A \times B| = ?$$
- $32$

> [!Answer]-
> - $32$
### Question 17
$$\text{Let } A = \{\{1, 2\}, 3\}. \text{ Which is true? (Select all that are correct)}$$
- $2 \in A$
- $\{3\} \in A$
- $1 \in A$
- $\{1, 2\} \in A$

> [!Answer]-
> - $\{1, 2\} \in A$
### Question 18
$$\text{Which implications are always true? (Select all that are correct)}$$
- $A \subseteq B \implies A \cup B = B$
- $A \cap B = A \implies A \subseteq B$
- $A \subseteq B \implies A \cap B = A$
- $A \cup B = A \implies B \subseteq A$

> [!Answer]-
> - $A \subseteq B \implies A \cup B = B$
> - $A \cap B = A \implies A \subseteq B$
> - $A \subseteq B \implies A \cap B = A$
> - $A \cup B = A \implies B \subseteq A$
### Question 19
$$\text{Let } B = \{\{a\}, a, \{a, b\}\}. \text{ Which statements are true? (Select all correct answers)}$$
- $\{a\} \in B$
- $a \in B$
- $b \in B$
- $\{a\} \subseteq B$
- $\{a, b\} \subseteq B$

> [!Answer]-
> - $\{a\} \in B$
> - $a \in B$
> - $\{a\} \subseteq B$
### Question 20
$$\text{How many students play either soccer or basketball?}$$
> [!Answer]-
> - $27$
### Question 21
$$\text{Let } A=\{1, \{1\}, \{2, 3\}, 4\}. \text{ Which of the following are elements of A? (Select all correct answers)}$$
- $1$
- $3$
- $\{1\}$
- $\{2, 3\}$
- $2$

> [!Answer]-
> - $1$
> - $\{1\}$
> - $\{2, 3\}$
### Question 22
$$\text{Let } C = \{\emptyset, \{\emptyset\}\}. \text{ Which are true? (Select all correct answers)}$$
- $\emptyset \in C$
- $\{\emptyset\} \in C$
- $\{\emptyset\} \subseteq C$
- $\{\{\emptyset\}\} \subseteq C$

> [!Answer]-
> - $\emptyset \in C$
> - $\{\emptyset\} \in C$
> - $\{\emptyset\} \subseteq C$
> - $\{\{\emptyset\}\} \subseteq C$
### Question 23
$$\text{If } A \cap B = \emptyset, \text{ which must be true? (Select all that are correct)}$$
- $A - B = A$
- $A = \emptyset \text{ or } B = \emptyset$
- $A \subset B$
- $B - A = B$

> [!Answer]-
> - $A - B = A$
> - $B - A = B$
### Question 24
$$\text{Let } |A| = 12, |B| = 9, |A \cap B| = 4. \text{ Find } |A \cup B|$$
- $21$
- $17$
- $25$
- $5$

> [!Answer]-
> - $17$
### Question 25
$$\text{Let } A=\{1, 2\}. \text{ Which are elements of } A \times A? \text{ (Select all that are correct)}$$
- $(1, 1)$
- $(2, 1)$
- $\{1, 2\}$
- $(1, 2)$
- $(2, 2)$

> [!Answer]-
> - $(1, 1)$
> - $(2, 1)$
> - $(1, 2)$
> - $(2, 2)$
### Question 26
$$\text{If } |U| = 40, |A| = 18, |B| = 20, |A \cap B| = 5, \text{ then } |(A \cup B)^C| = ?$$
> [!Answer]-
> - $7$
### Question 27
$$\text{If } A \subseteq B \text{ and } B \subseteq C, \text{ which must be true?}$$
- $A \subseteq C$
- $C \subseteq A$
- $A = C$
- $A \subset C$

> [!Answer]-
> - $A \subseteq C$
### Question 28
$$(A \cap B) \cup A = A$$
- True
- False

> [!Answer]-
> - True
### Question 29
$$\text{Let } A=\{1, 2, 3\} \text{ and } B=\{1, 2, 3, 4\}. \text{ Which are true (Select all correct answers)}$$
- $A \subset B$
- $A = B$
- $A \subseteq A$
- $A \subseteq B$
- $B \subseteq A$

> [!Answer]-
> - $A \subset B$
> - $A \subseteq A$
> - $A \subseteq B$