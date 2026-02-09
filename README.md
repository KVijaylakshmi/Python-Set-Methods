# Python-Set-Methods
A Set in Python is a collection of unique elements which are unordered and mutable. Python provides various functions to work with Set. In this article, we will see a list of all the functions provided by Python to deal with Sets.

# Adding and Removing elements
We can add and remove elements form the set with the help of the below functions - 

add(): Adds a given element to a set
clear(): Removes all elements from the set
discard(): Removes the element from the set
pop(): Returns and removes a random element from the set
remove(): Removes the element from the set
Example: Adding and removing elements from the Set.

Creating a set
fruits = {"apple", "banana", "cherry"}

1. add() – add one element
fruits.add("orange")
print(fruits)

2. update() – add multiple elements
fruits.update(["mango", "grape"])
print(fruits)

3. remove() – remove an element (raises error if not found)
fruits.remove("banana")

4. discard() – remove an element (no error if missing)
fruits.discard("banana")  # safe

5. pop() – remove and return a random element
item = fruits.pop()
print(item)

6. clear() – remove all elements
fruits.clear()
print(fruits)  # set()

Set Operations (the fun part 😎)
A = {1, 2, 3, 4}
B = {3, 4, 5, 6}

7. union()
print(A.union(B))        # {1, 2, 3, 4, 5, 6}
# or
print(A | B)

8. intersection()
print(A.intersection(B)) # {3, 4}
# or
print(A & B)

9. difference()
print(A.difference(B))   # {1, 2}
# or
print(A - B)

10. symmetric_difference()
print(A.symmetric_difference(B))  # {1, 2, 5, 6}
# or
print(A ^ B)

11. issubset() / issuperset()
C = {1, 2}
print(C.issubset(A))     # True
print(A.issuperset(C))  # True

12. isdisjoint() – no common elements?
print(A.isdisjoint({7, 8}))  # True
