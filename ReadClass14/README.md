# Read Class 14

**Intro to password hashing:**

1. **Define the term “hashing”:** Hashing is the process of transforming a piece of data (such as a password) into a fixed-length string of characters (called a hash or a digest) using a mathematical function (called a hash function) that is hard to reverse.

2. **Explain to a non-technical friend what a hash function does to a password:** A hash function does to a password what a blender does to a fruit. It takes the password as an input and produces a hash as an output. The hash is like a smoothie that has no trace of the original password. You cannot get the password back from the hash, just like you cannot get the fruit back from the smoothie. The hash function also makes sure that every password has a unique hash, so no two passwords can produce the same smoothie.

**bcrypt overview:**

1. **What does it mean to 'salt' a password?** Salting a password means adding some random data (called a salt) to the password before hashing it. This makes the hash more secure and harder to crack by brute force or dictionary attacks. The salt is usually stored along with the hash in the database.

2. **What piece of information would a hacker need to access in order to find the 'salt' string for your passwords?** A hacker would need to access the database where the hashes and salts are stored in order to find the salt string for your passwords. The salt is usually appended or prepended to the password before hashing, so the hacker would need to know how the salt is combined with the password.

**jBCrypt (Blowfish-based hashing):**

1. **How does the Blowfish block cipher handle the increased computation speed of new computers?** The Blowfish block cipher handles the increased computation speed of new computers by using a variable number of rounds (from 4 to 31) in its encryption algorithm. The more rounds, the more secure the encryption, but also the more time it takes. The number of rounds can be adjusted according to the security needs and performance requirements.

2. **What are the issues with the two most common password hashes for Java (“Java password hash” and “Java password encryption”)?** The two most common password hashes for Java are MD5 and SHA-1. Both of them have serious security issues and should not be used for password hashing. MD5 is vulnerable to collision attacks, which means that two different passwords can have the same hash. SHA-1 is also weak against collision attacks and has been officially deprecated by NIST. Both MD5 and SHA-1 are also fast to compute, which makes them easy to crack by brute force or dictionary attacks.
