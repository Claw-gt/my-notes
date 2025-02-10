Password file: */etc/passwd* it contains the password hash => Vulnerable to password cracking since an attacker could use brute force attack until getting the same hash

**Mitigation:**
- Remove Passwords hashes for the file, they will be in the */etc/shadow* file instead (Shadow file can be locked down and highly restricted so that only root can access it)

##### Types of Attacks

**Brute Force Attacks**: Try all possibilities
**Dictionary Attacks**: Try English words first
**Hybrid Attacks**: Add variations to tries
**Rainbow Table Attacks**: Precomputes hashes
**Password Spraying**: Exploits common passwords and uses them in different accounts => *prohibit* the use of common passwords
**Credential Stuffing**: Exploits reused passwords => use *password manager* to generate and maintain *unique passwords* and *MFA*

`$> unshadow` => combines the original password file and the contents of the shadow file into a single file

Tool for password cracking: *John The Ripper*