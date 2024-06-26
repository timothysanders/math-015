# Chapter 2: Sets and Counting

## 2.1 Sets and Set Operations
### Set Notation
- *Roster method* is listing the members of a set
  - "set consisting of ..."
  - Written as `{x, y, z}`
  - Can use `...` to indicate "and so on" in the pattern that has been established
  - Each distinct element is only listed once, order of elements does not matter
- *Set-Builder Notation*
  - Example notation `{X | X < 6, X ∈ positive integers}`
    - "set of all numbers that we are calling x, such that x is less than six, and x in an element of positive integers"
    - Equivalent form in roster method of notation would be `{1, 2, 3, 4, 5}`
  - `|` means "such that"
  - `∈` means "member of/is an element of"
  - `∉` means "not a member of/is not an element of"
  - `∋` means "contains as member"
  - `∌` means "does not contain as member"
  - Certain sets will be "out of bounds" of the roster method
    - For example, "real numbers between 4 and 5" is technically infinite, so cannot be listed in the roster method
  - "real numbers greater than four"
    - `{X | X > 4, X ∈ real numbers}`
  - "integers less than -2"
    - `{X | X < -2, X ∈ integers}`
  - "real numbers between -2 and 5"
    - `{X | 5 > X > -2}`
  - Real numbers are considered to be included in set builder notation by default, so no need to explicitly notate it
  - Whatever is on the left side of the "such that" line (`|`) is the general type of thing in the set
- By tradition, sets are notated with capital letters
- Cardinal number of set is the number of elements in the set
  - For example, in set R, where `R = {r, a, m, o, n, e, s}`, then `n(R) = 7`
  - Also in set R, `m ∈ R` and `x ∉ R`
- Two sets are considered equal if they contain exactly the same elements
  - Note that order doesn't matter
- When sets are not appropriate to describe with roster notation, can use set builder notation
- `ℝ` is used to notate "set of real numbers"
- `∅` is used to notate an "empty set"
### Definitions
- `set`: collection of objects, things, numbers
- `elements/members`: objects or things in a set
- `well defined set`: sets where there is a particular way of determining for sure whether or not an item is a member of a set
- `roster notation/listing notation`: method of describing a set by listing each element of the set inside the symbols `{}`
- `set-builder notation`: lists the rules that determine whether an object is an element of the set rather than the actual elements
- `cardinal number`: number of elements in the set, if A is the set, notated with `n(A)`
- `empty set`: a set with no elements, notated with `∅`

### Universal Set and Subsets
- When working with sets, you must define a universal set, notated with `U`
  - For example, when spelling words, the universal set is all letters of the alphabet
- When all elements of one set are also members of another set, we call the first set a subset of the second set
- Proper subsets are notated with `⊂`
  - If A is a subset of B, we would notate as `A ⊆ B`
- Subset or equal is notated with `⊆` (this seems to also be used just to mean "subset")
- Sets that are not a proper subset of another, then it is notated as `⊈`
  - For example, if A contains an element that is not in B, then `A ⊈ B`
- Complement of a set A is all elements that are in the universal set, but not in set A
  - Also, sometimes called "prime"
  - Notated like `A'` ("A prime")
- Complement of the universal set is an empty set
- Complement of an empty set is the universal set
- If A = `{2, 4, 6, 8, 10}`, B = `{4, 6}`, C = `{2, 3, 4}`
  - `B ⊆ A`
  - `C ⊈ A`
- Empty set is a subset of every set
- Proper subset means that every element of one set B is in another A and that A contains something not in B
  - The two sets are not equal
- Venn Diagrams can be used to notate sets as well
  - Box around the circles is the "universal set", with each circle representing the individual sets
- All subsets of `{1, 2, 3}`
  - Empty set is a subset
  - `{1}, {2}, {3}, {1, 2}, {1, 3}, {2, 3}, {1, 2, 3}`
  - All subsets except for `{1, 2, 3}` are proper subsets `⊆`
  - Number of subsets can be found by calculating `2^n` where `n` equals number of elements
  - Number of subsets grows exponentially with number of elements
### Definitions
- `universal set`: set of all possible elements in any set used in the problem
- `subset`: a set where all elements are members of another set
- `natural numbers`: integers 1, 2, 3, 4, ... (excludes zero)
- `whole numbers`: including 0, integers 1, 2, 3, 4, ...
- `proper subset`: a subset B of another set A, where A contains elements outside of B
- `improper subset`: a subset B where B contains every element of set A
- `integers`: set of numbers which contains `..., -3, -2, -1, 0, 1, 2, 3,...`
- `rational numbers`: all numbers that can be written in the form of a fraction
- `irrational numbers`: all numbers than cannot be written in the form of a fraction
- `real numbers`: the superset of rational and irrational numbers

### Intersection of Sets
- Intersection is the part of sets that are shared, notated `∩`
  - Another way to phrase this is "elements in both A and B"  
  - Given `A = {1, 2, 3}` and `B = {3, 4, 5}`, then `'A ∩ B = {3}`
  - An intersection of two sets that has no members is the empty set, these sets are then called "disjoint"
  - Using set builder notation, `A ∩ B = {X | X ∈ A and X ∈ B}`
- Union is the combination of multiple sets, notated with `∪`
  - For example, `A ∪ B = {1, 2, 3, 4, 5}`
### Definitions
- `intersection`: all elements in A and B, the overlap of the two sets
- `union`: all elements in A or B, elements in either set, or both

### Mutually Exclusive Sets
- Pairs of sets may have no overlaps
- `A ∩ B = ∅` 
### Definitions
- `mutually exclusive/disjoint`: sets with no elements in common

### Union of Sets
- In logic and mathematics, using or means an inclusive or, unless specified otherwise
- `A ∪ B = {X | X ∈ A or X ∈ B}`
- Because union is elements that are in both sets, to find `n(A ∪ B)`, we need to add `n(A)` + `n(B)`, then subtract the cardinal number of `A ∩ B`
### Definitions
- `union`: new set formed by joining two sets together, all elements in one set or the other or both

### Complement of a Set
- Universal set is all elements under consideration
- Complement of a set is all of the elements of the universal set that are outside of the set under consideration
  - Notated by `A'` ("A prime")
  - `A' = {X | X ∈ U and X ∉ A}`
- Complement of the universal set is an empty set, complement of an empty set is the universal set
- No element of the universal set can be in both A and A' at the same time
  - Sum of cardinal numbers of A and A' is the cardinal number of U
- Cardinal number rule for the complement of a set
  - `n(A) + n(A') = n(U)`
  - `n(A) = n(U) - n(A')`
  - `n(A') = n(U) - n(A)`

### Set Theory & Logic
- Logic involves using English sentences called "statements", must be able to be True or False, but not both
- Compound statements are multiple statements put together
  - "If/Then" is a particular kind of compound statement
  - "Or" is another kind of compound statement
- Statements are often designated with `p` and `q`
- Negation = "not" = `~p`
- Conjunction = "and" = `∧`
- Disjunction = "or" = `∨`
- Conditional = "If...then" = `→`
- Biconditional = "If and only if" = `<->`
- Set theory and logic have many similarities
  - For example, union and disjunction are the same meaning, but used in different circumstances

| Set Theory   | Logic       | Common Wording  |
|--------------|-------------|-----------------|
| union        | disjunction | or              |
| intersection | conjunction | and             |
| complement   | negation    | not             |
| subset       | conditional | if ... then ... |

## 2.2 Applications of Venn Diagrams
### Surveys
- Surveys are often used to divide people and objects, but categories often overlap and people are in more than one category
- Solving a cardinal number problem
  - Define a set for each category in the universal set
  - Draw a Venn diagram with as many overlapping circles as number of sets
  - Write down all given cardinal numbers for each set
  - Starting with innermost overlap, fill in each region of Venn diagram
- "Union/Intersection Rule"
  - `n(T ∪ C) = n(T) + n(C) - n(T ∩ C)`

### De Morgan's Laws
- Basic property of algebra is the distributive property
  - `a(b + c) = ab + ac`
  - Operation outside of the parentheses (a) is distributed to the operation inside the parentheses
- Relationship of `(A ∪ B)' = A' ∩ B'` is known as one of De Morgan's Laws
  - That is, the complement of a union is the intersection of the complements
- Additionally `(A ∩ B)' = A' ∪ B'`
  - That is the complement of an intersection is the union of the complements
- To find the intersection of two sets
  - Given `n(A) = 15, n(B) = 32, n(A ∪ B) = 41`
  - `n(A ∪ B) = n(A) + n(B) - n(A ∩ B)`
  - `41 = 15 + 32 - n(A ∩ B)`
  - `n(A ∩ B) = 6`

## 2.3 Introduction to Combinatorics
### The Fundamental Principle of Counting
- Also known as the "counting principle"
- Number of items in a sample space is important
- Multiply number of possibilities of each part in an overall experiment
  - For example, how many combinations might there be of a coin toss combined with rolling a die?
    - We would multiply the coin toss outcomes (2) by the number of dice outcomes (6) = 12
- Certain solutions are meant for problems "without replacement" vs. "with replacement"
- How many 3-digit area codes are possible if the first digit cannot be 0?
  - Because we cannot have a zero at the beginning, we would multiple the following
    - 9 * 10 * 10 = 900
- Tree diagrams can also be used to identify possible combinations of choices/outcomes
  - However, this method is very time-consuming and impractical for larger problem sets
  - A shortcut method is desirable instead
- If you have two pairs of jeans, three shirts, and two pairs of shoes, how many outfits can you make?
  - 2 * 3 * 2 = 12 outfits
### Definitions
- `tree diagram`: a diagram consisting of clusters of line segments, or branches
- `fundamental principle of counting`: total number of possible outcomes of a series of decisions found by multiplying the number of choices for each decision/category

### Factorials
- Factorials are notated as `n!`
  - For example, `3! = 3 * 2 * 1 = 6`
  - `4! = 4 * 3 * 2 * 1`
  - `0! = 1` - this is a special case
  - `8! = 8 * 7!`
- Can use factorial notation for some division problems as well
  - `9!/6!` can be also represented as `(9 * 8 * 7 * 6!)/6!`
  - `6!` cancels out and we are left with `9 * 8 * 7 = 504`
- If n is a positive integer, then n factorial is notated like `n!` and is the product of all positive integers less than or equal to n
### Definitions
- `Pascal's Triangle`: gives you the coefficients of an expansion of a binomial

## 2.4 Permutations & Combinations
- Fundamental principle of counting allows you to determine the total number of possible outcomes when a series of decisions needs to be made
- This can also be applied to scenarios where more than one item is selected from each category

### With vs Without Replacement
- Selecting items "with replacement" means the same item can be picked more than once
- Selecting items "without replacement" means the same item cannot be picked more than once
- When selecting items without replacement, permutations and combinations are used to determine total possible outcomes

### Permutations
- When more than one item is selected without replacement from a category, and the order is important, these outcomes are called permutations
- Permutation is putting a group of things in order, if order matters, it is a permutations
- Order is always important in permutations
- Permutation notation can be written as `P(n,r)` 
  - Formula is `n!/(n-r)!`
  - `P(8,3)` translates to `8!/(8-3)!`
  - In this formula, `n` is the number of elements in the pool and `r` is the number of elements selected
- Example, six bands who will be playing in four slots `P(6,4)`
  - `6!/(6-4)! = 6 * 5 * 4 * 3 = 360`
- Example, 112 attendees and three prizes `P(112,3)`
  - `112!/(112-3)! = 112 * 111 * 110 = 1,367,520`
### Definitions
- `permutation`: arrangement of objects in a definite order

### Combinations
- If the order of selections is not important, then those possible outcomes are called "combinations"
- Combinations groupings of things, if order does not matter, then it can be a combination
- Combination notation can be written as `C(n,r)`
- When `r` items are selected from a pool of `n` items
  - Formula is `n!/r!(n-r)!`
  - Note that this formula only works when items are selected without replacement
  - Example, five DVDs from a group of fifty
    - `C(50,5)`
    - `50!/5!(50-5)!` -> `50!/5!45!` -> `50*49*48*47*46/5*4*3*2*1`
  - Example, five card poker hands?
    - `C(52,5)`
    - `52!/5!(52-5)!` -> `(52*51*50*49*48*47)/(5*4*3*2*1)`
- When calculating combinations of groups, you can multiply them together
  - Example, select five-person committee from 12 women and 9 men
    - Must contain 3 women and 2 men
    - `C(12,3) * C(9,2)` -> `220 * 36 = 7920`
    - Any combination of people
    - `C(21,5) = 20349`
- Important aspect of combinatorics is deciding which technique to use
  - Can selected items be repeated? -> Fundamental Principle of Counting
  - If more than one category...
    - And order of items matters -> Use permutations
    - And order of items doesn't matter -> Use combinations
  - If order of selections does not matter -> Use combinations
  - If order of selections does matter -> Use permutations
### Definitions
- `combination`: order is not important, words like group, team, and committee are often used
- `pascal's triangle`

### Permutations of Identical Items
- For example, how many different ways can the letters of SEE be arranged?
  - Note that two letters are identical
  - `n!/x!` where `n` is the number of letters (in SEE) and `x` is the number of identical letters
- Dividing by the factorial of the repeated letter eliminates the duplicate arrangements
- This formula can be extended
  - For example, `n!/x!y!z!...`
### Definitions
- `distinguishable permutations`: 