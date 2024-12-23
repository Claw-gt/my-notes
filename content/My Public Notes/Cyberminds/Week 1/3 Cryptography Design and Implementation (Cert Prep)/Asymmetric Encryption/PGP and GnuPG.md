### *Pretty Good Privacy*
- Phil Zimmerman
- OpenPGP is commonly used

> [!info]
> **Framework to use other encryption algorithms**
> Symmetric + Asymmetric encryption

```mermaid
flowchart TD
subgraph encryption
Data --> Generate_SymmetricKey --SymmetricKey --> EncryptData
EncryptData --PublicKeyRSA --> Encrypt_SymmetricKey
end
subgraph decryption
EncryptedMessage --Receiver_PrivateKeyRSA --> Decrypt --> SymmetricKey
SymmetricKey --DecryptMessage --> Message
end
```

### *GnuPG*
Open-source implementation of PGP
