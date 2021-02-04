# Hash Table 

## What is Hash Table?
Hash Table(also called Hash Map) is one of Hash-based structures. It looks similar to arrays -- we map index to values, but for Hash Table, we use keys instead of indexes.

## Why it's that fast?
What happens behind the scene is that a Hash Table uses a hash function to compute an index from the key, and the index tells which array of buckets the value should be stored into. Therefore when we want to find where the value is stored, we can compute the index with the hash function and find out where the desired value is stored.

![/](https://res.cloudinary.com/practicaldev/image/fetch/s--Bs4o-sMk--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/tnkyfmooafebqeyr2eye.png)

## Dealing with collisions

### Method 1: Separate Chaining

With Separate Chaining, we store them at the same bucket nesting another sort of list inside. If it's implemented with Linked List or Array, lookup time will depend on the average number of keys per bucket. 


### Method 2: Linear Probing 

Linear Probing is one of Open Addressing strategy, and with Open Addressing Strategy, we only allow one key-value set per bucket. When we find a collision, we search through the array until we find an unoccupied bucket.