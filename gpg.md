# GPG and gnupg Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

## Table of Contents
- [Introduction](#introduction)
- [Key Generation](#key-generation)
- [Key Management](#key-management)
- [Encryption](#encryption)
- [Decryption](#decryption)
- [Signing](#signing)
- [Verification](#verification)
- [Revocation](#revocation)
- [Additional Resources](#additional-resources)

## Introduction
- Explanation of GPG and gnupg
- Importance of encryption and digital signatures

## Key Generation
- Generating a new key pair
    - `gpg --gen-key`
- Choosing key types and sizes
    - `gpg --full-gen-key`
- Setting key expiration dates
    - `gpg --edit-key KEYID`

## Key Management
- Listing existing keys
    - `gpg --list-keys`
- Importing and exporting keys
    - `gpg --import FILE`
    - `gpg --export KEYID`
- Deleting keys
    - `gpg --delete-key KEYID`
- Changing key trust levels
    - `gpg --edit-key KEYID`

## Encryption
- Encrypting files and messages
    - `gpg --encrypt --recipient RECIPIENT FILE`
- Encrypting for multiple recipients
    - `gpg --encrypt --recipient RECIPIENT1 --recipient RECIPIENT2 FILE`
- Encrypting with symmetric encryption
    - `gpg --symmetric FILE`

## Decryption
- Decrypting files and messages
    - `gpg --decrypt FILE`
- Decrypting with a passphrase
    - `gpg --decrypt --passphrase PASSPHRASE FILE`
- Decrypting with a private key
    - `gpg --decrypt --recipient KEYID FILE`

## Signing
- Creating a digital signature
    - `gpg --sign FILE`
- Signing files and messages
    - `gpg --sign --local-user KEYID FILE`
- Signing with multiple keys
    - `gpg --sign --local-user KEYID1 --local-user KEYID2 FILE`

## Verification
- Verifying digital signatures
    - `gpg --verify FILE`
- Verifying signed files and messages
    - `gpg --verify FILE.sig FILE`
- Verifying with multiple keys
    - `gpg --verify --keyring KEYRING FILE`

## Revocation
- Revoking a key
    - `gpg --edit-key KEYID`
    - `revkey`
- Generating a revocation certificate
    - `gpg --gen-revoke KEYID`
- Importing a revocation certificate
    - `gpg --import FILE`

## Additional Resources
- Links to official documentation
- Useful tutorials and guides
- Recommended books and articles
