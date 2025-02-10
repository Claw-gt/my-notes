## Brute Force Attacks
Repeatedly guess keys
Brute-force attacks are also called as **know ciphertext attacks** (the attacker only needs the ciphertext)
=> Modern algorithms aren't susceptible to brute-force attacks
=> Flawed algorithms may be vulnerable to brute-force attacks (weak implementation of a moder cryptographic system that limtis keyspace)
##### Keyspace
The set of all possible encryption keys usable with an algorithm

## Knowledge-based Attacks

##### Frequency Analysis
Detects patterns in ciphertext (e.g. common letters in English)
##### Known Plaintext Attack
Analysts have acces to unencrypted and encrypted text
Attacker uses this knowledge to retrieve the decryption key for other messages
##### Chosen Plaintext Attack
Attacker can create an encrypted message of their choice
##### Birthday Attack
Attacker finds two inputs with the same hash values
23 people in a room => 50% chance that two people share birthday
70 people in a room => 99,9% chance ""

## Limitations of encryption algorithms
Every encryption algorithm has some weakness

- Some algorithms are faster than others (symmetric faster than asymmetric)
- The longer the key, the more computing power they need => slower
- Some key choices may have inhenret flaws
- Reusing the same key facilitates cryptanalytic attacks
- Cryptographic algorithms and keys have limited longevity (limited by math and computing power)
- **Downgrade attacks** remove or weaken encryption (e.g POODLE attack)
*Entropy* reduces the predictability of cryptographic methods