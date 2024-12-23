# Key Escrow
Third party holding encryption keys
Allows government access to keys
e.g Clipper chip
- Privacy controversy

# Key Stretching

Takes a relatively insecure value, such a password, and uses mathematical techniques to strengthen it, making it harder to crack

### Process

**1. Salting**
Encryption Key + Salt 
**2. Hashing**
Adds time to the verification process by requiring more math

### Algorithm for Key Stretching

**PBKDF2** -> Password-Based Key Derivation Function v2
--> Salting (at least 4000 times) + Hashing
**bcrypt** -> with Blowfish