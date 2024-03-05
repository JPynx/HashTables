# HashTables

# Which is a better hash function:
1. x % n where n is a large number with several factors
2. x % n where n is a large prime number
   In general, using a large prime number for the modulus operation in a hash function usually leads to better randomness and fewer collisions compared to using a non-prime number with multiple factors. However, the best choice depends on factors like the type of data and how evenly you want the keys to be distributed.
# Is char values summed % 599 a good hash function for strings? Why or why not?
  Summing character values modulo 599 is a simple and efficient hash function for strings. However, its effectiveness varies depending on the strings and the application's 
  needs. It might work fine in some situations but could lead to uneven distribution and collisions in others.
# Take a look at Java's HashMap class and how it produces hashed values, then describe how it works. 
"HashMap use singly linked list to store elements, these are called bins or buckets. When we call put method, hashCode of key is used to determine the bucket that will be used to store the mapping. "
