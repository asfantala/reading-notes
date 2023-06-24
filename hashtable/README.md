# HashTables 

### What is Hashtables ?
- A hash table is a data structure that is used to store keys/value pairs.
- is a data structure that provides efficient lookup, insertion, and deletion operations.
- It uses a hash function to compute an index into an array of buckets or slots, from which the desired value can be found.
- The hash function will assign each key to a unique bucket, but multiple keys may be assigned to the same bucket.
- Hash tables are commonly used in data structures such as maps and sets.
- Hash tables are commonly used because they are very efficient for finding and retrieving data.
- The main advantage of using a hashtable is its constant-time average-case complexity for basic operations, such as insertion, deletion, and retrieval.
### How does it work? 
- The key of the item you want to retrieve
- The hash code of that key, which is computed using a hash function
- The index, which is the hash code modulo the length of the array
- The value at that index if it exists, or null otherwise.

### Structure
- Hashing is implemented in two steps:
  - An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
  - The element is stored in the hash table where it can be quickly retrieved using hashed key.

### Methods 
- Add()
- Get()
- Hash()
- GetHash()
- GetHashKey()
- GetHashValue()
- Keys()






