## **Hash Tables**

### ***What is Hashing?***

- Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects. In the case of a hashtable, it is used to determine the index of the array.

### ***Why do we use them?***

1. Hold unique values
2. Dictionary
3. Library

>In universities, each student is assigned a unique roll number that can be used to retrieve information about them.

>In libraries, each book is assigned a unique number that can be used to determine information about the book, such as its exact position in the library or the users it has been issued to etc.

- In hashing, large keys are converted into small keys by using `hash functions`. The values are then stored in a data structure called `hash table`. The idea of hashing is to distribute entries `key/value pairs` uniformly across an array.

### ***What Are they***

- The basic idea of a hashtable is the ability to store the `key` into this data structure, and quickly retrieve the `value`. This is done through what we call a `hash`. A `hash` is the ability to encode the key that will eventually `map` to a specific location in the data structure that we can look at directly to retrieve the `value`.

- Since we are able to `hash` our `key` and determine the exact location where our `value` is stored, we can do a lookup in an `O(1)` time complexity. 

### ***Hash function***

- A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The `values returned by a hash function` are called `hash values, hash codes, hash sums, or simply hashes`. 

- The `hash code` is used again to read something from the `hash map`. Take the `key`, run it through the `hash code` to get a number, use that number to `index the array`.

### ***Steps to  implemented  Hashing***

1.  An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.


### ***Buckets***
 - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

### ***Collisions***
 - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

- Collisions are solved by changing the initial state of the` buckets`. Instead of starting them all as `null` we can initialize a `LinkedList` in each one

### ***Creating a Hash***

- A hashtable traditionally is created from an `array`, it's like the size `1024`. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that `key` into a numeric number value. 

1. Add or multiply all the ASCII values together.
2. Multiply it by a prime number such as 599.
3. Use modulo to get the remainder of the result, when divided by the total size of the array.
4. Insert into the array at that index.

>Example:

Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16

Key gets placed in index of 16. 

>We now know that our `key Cat` maps to `index 16` of the array. We can view into this index and find `Josie, our value` quickly.


### ***Hash maps do this to store values***

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- store the key with the value by appending both to the end of a linked list

### ***Hash maps do this to read value:***

- accept a key
- calculate the hash of the key
- use modulus to convert the hash into an array index
- use the array index to access the short LinkedList representing a bucket
- search through the bucket looking for a node with a key/value pair that matches the key you were given



### ***Internal Methods***
- **Add()**:
 - When adding a new key/value pair to a hashtable:
  1. send the key to the GetHash method.
  2. Once you determine the index of where it should be placed, go to that index
  3. Check if something exists at that index already, if it doesn???t, add it with the key/value pair.
  4. If something does exist, add the new key/value pair to the data structure within that bucket.

- **Find()**
  - The Find takes in a `key`, gets the Hash, and goes to the `index` location specified. Once at the `index` location is found in the array, it is then the responsibility of the algorithm the iterate through the `bucket` and see if the `key exists` and return the `value`.

- **Contains()**
  - The Contains method will accept a `key`, and return a `bool on` if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the `key` exists in the table given the `index` returned.

- **GetHash()**
  - The GetHash will accept a `key` as a string, conduct the `hash`, and then return the `index` of the array where the `key/value` should be placed.


-------------------------------------------------------------



**References:**

@By codefellows/[Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html) 

@By hackerearth/[Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)

