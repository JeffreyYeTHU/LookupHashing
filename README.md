# Lookup Hashing
The basic info you need to know about lookup hashing.

## What is hashing?
Hashing is the process of converting a given key into another value. A __hash function__ is used to generate the new value according to an algorithm. The result of a hash function is know as __hash value__, or simply, __hash__.

For instance, suppose we have a hash function $h(x) = x mod 5$, when $x=13$, the __hash value__ is 3.

## Collision
If two keys generate the same hash, it is called collision. Continued with earlier example, $x=13$ and $x=23$ will both have hash of __3__, so it is a collision.

## Lookup hashing vs encryption hashing
Hashing most commonly used to implement __hash tables__. A hahs table store key/value pairs in the form of a list where any element can be accessed by it's key. When using in this scenario, it is __lookup hashing__. This [hash table video](https://www.youtube.com/watch?v=KyUTuwz_b7Q) done a really good job on explain the basics of construct a hash table.

Hashing is also commonly used in encryption. __MD5, SHA-1, SHA-2__ are some popular encryption hashes.

## Commonly used lookup hashing
Here is a [hash algorithm blog](https://eternallyconfuzzled.com/hashing-c-introduction-to-hashing/)  that explain some basic lookup hashing algorithm.

For lookup hashing, the key is to have good distribution so to avoid collision. In this project, I will exam 3 algorithm and test their hashing ability.
* Bernstein hash
* Modified Bernstein
* Somewhat mixture of the above two

The third one inspired by [this link](https://stackoverflow.com/questions/263400/what-is-the-best-algorithm-for-overriding-gethashcode).

