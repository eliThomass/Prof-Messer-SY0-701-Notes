# Quiz 1.4 — Public Key Infrastructure
*Professor Messer SY0-701 · Section 1.4*

---

### 1. What is a key characteristic of symmetric encryption?
- [ ] It uses two mathematically related keys
- [ ] It uses a single, shared key to both encrypt and decrypt
- [ ] It cannot be combined with asymmetric encryption
- [ ] It scales easily to large numbers of users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It uses a single, shared key to both encrypt and decrypt</p>
<p>Symmetric encryption uses a single shared key: encrypt with the key, decrypt with the same key. It's fast with less overhead, but doesn't scale well since the key is hard to distribute.</p>
</details>

---

### 2. In asymmetric encryption, if data is encrypted with someone's public key, what is required to decrypt it?
- [ ] Their private key
- [ ] The same public key
- [ ] A shared symmetric key
- [ ] The Certificate Authority's key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Their private key</p>
<p>The private key is the only key that can decrypt data encrypted with the matching public key — e.g. encrypt a message to Bob with his public key, and only Bob's private key can decrypt it.</p>
</details>

---

### 3. What is key escrow?
- [ ] Encrypting a database column with its own key
- [ ] A third party (or your own organization) holding a copy of your private keys
- [ ] Replacing sensitive data with a non-sensitive token
- [ ] Rotating cryptographic keys automatically

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A third party (or your own organization) holding a copy of your private keys</p>
<p>Key escrow means someone else holds your decryption keys — a 3rd party, or done internally within your own organization. It's controversial, but sometimes required for data availability.</p>
</details>

---

### 4. Tools like BitLocker and FileVault are used for what kind of encryption?
- [ ] Column-level database encryption
- [ ] Full disk / partition encryption
- [ ] Transport encryption
- [ ] Tokenization

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Full disk / partition encryption</p>
<p>BitLocker and FileVault provide full disk and partition encryption to protect data on storage devices.</p>
</details>

---

### 5. What does transparent database encryption do?
- [ ] Encrypts each column with its own individual symmetric key
- [ ] Encrypts all database information with a single symmetric key
- [ ] Masks data only from view based on permissions
- [ ] Replaces database values with tokens

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Encrypts all database information with a single symmetric key</p>
<p>Transparent encryption encrypts all database info with a symmetric key, as opposed to column-level (record-level) encryption where each column has its own symmetric key.</p>
</details>

---

### 6. A site-to-site VPN connecting two office networks typically uses which technology?
- [ ] SSL/TLS
- [ ] IPsec
- [ ] SHA-256
- [ ] OCSP

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> IPsec</p>
<p>Client-based VPNs use SSL/TLS, while site-to-site VPNs use IPsec to encrypt all data transmitted over the network.</p>
</details>

---

### 7. What is "key stretching"?
- [ ] Increasing the length of a symmetric key to 3072 bits
- [ ] Performing the encryption/hashing process multiple times on the same data
- [ ] Sharing a key out-of-band via courier or phone
- [ ] Combining a private key with someone else's public key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Performing the encryption/hashing process multiple times on the same data</p>
<p>Key stretching performs the process multiple times on data — for example, hashing the hash of the hash of a password.</p>
</details>

---

### 8. In public key cryptography key exchange, how do Bob and Alice arrive at the same symmetric key without ever transmitting it?
- [ ] They both send their private keys to a Certificate Authority
- [ ] Bob combines his private key with Alice's public key, and Alice combines her private key with Bob's public key
- [ ] They exchange the key out-of-band by phone
- [ ] They use the same salt value

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Bob combines his private key with Alice's public key, and Alice combines her private key with Bob's public key</p>
<p>This produces the same symmetric key for both sides without ever sending anything sensitive across the network — an in-band key exchange technique.</p>
</details>

---

### 9. Which hardware component is a cryptographic processor typically built into a single device (like a laptop) to store keys and passwords?
- [ ] Hardware Security Module (HSM)
- [ ] Trusted Platform Module (TPM)
- [ ] Key management system
- [ ] Secure Enclave

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Trusted Platform Module (TPM)</p>
<p>A TPM is hardware specifically designed for cryptographic functions, with persistent/versatile memory, and is usually used for a single device.</p>
</details>

---

### 10. Which technology is used in large environments like server clusters to securely store thousands of cryptographic keys with hardware acceleration?
- [ ] Trusted Platform Module (TPM)
- [ ] Hardware Security Module (HSM)
- [ ] Secure Enclave
- [ ] Wildcard certificate

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Hardware Security Module (HSM)</p>
<p>HSMs are used in large environments like server clusters, securely storing thousands of keys with high-end hardware, key backup, and cryptographic accelerators.</p>
</details>

---

### 11. What is a Secure Enclave?
- [ ] A centralized service that manages keys across cloud providers
- [ ] A separate hardware processor on a device that keeps secrets private even if the device is compromised
- [ ] A list of revoked certificates maintained by a CA
- [ ] A shared key held in escrow by a third party

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A separate hardware processor on a device that keeps secrets private even if the device is compromised</p>
<p>A Secure Enclave is implemented as its own hardware processor (separate from the main processor) with its own boot ROM, true RNG, real-time memory encryption, and root cryptographic keys.</p>
</details>

---

### 12. Hiding a secret message inside an image or audio file is an example of what?
- [ ] Tokenization
- [ ] Data masking
- [ ] Steganography
- [ ] Key escrow

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Steganography</p>
<p>Steganography is security through obscurity — hiding info in plain sight, such as embedding a message inside an image, audio, video, or TCP packets (the covertext).</p>
</details>

---

### 13. Replacing a credit card number with a random substitute value that has no mathematical relationship to the original is called what, and is explicitly NOT encryption or hashing?
- [ ] Tokenization
- [ ] Steganography
- [ ] Key stretching
- [ ] Salting

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Tokenization</p>
<p>Tokenization replaces sensitive data with a non-sensitive token — common with credit card processing — and is specifically not encryption or hashing.</p>
</details>

---

### 14. Showing only the last four digits of a bank card number on a printed receipt is an example of what?
- [ ] Data masking
- [ ] Tokenization
- [ ] Steganography
- [ ] A digital signature

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data masking</p>
<p>Data masking hides part of the original data (like showing only the last 4 digits of a card number) to protect PII, and may control the view based on permissions.</p>
</details>

---

### 15. What is a hash collision?
- [ ] When a hash cannot be reversed back into the original message
- [ ] When two different inputs produce the same hash output
- [ ] When a salt is reused across multiple passwords
- [ ] When a digital signature fails verification

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> When two different inputs produce the same hash output</p>
<p>A hash should always be unique for a given input. If different inputs create the same hash, that's a collision — these should be extremely rare.</p>
</details>

---

### 16. Why is a random salt added to a password before hashing it for storage?
- [ ] To make the hash reversible for password recovery
- [ ] To make rainbow table attacks ineffective and slow down brute-force attempts
- [ ] To allow the company to recover the original plaintext password
- [ ] To shorten the resulting hash value

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To make rainbow table attacks ineffective and slow down brute-force attempts</p>
<p>Every user gets their own random salt, so the same password produces a different hash per user. Rainbow tables don't work against salted hashes, and it slows down brute-force attacks.</p>
</details>

---

### 17. A digital signature is created by signing a document with which key, and verified with which key?
- [ ] Signed with the sender's public key; verified with the sender's private key
- [ ] Signed with the sender's private key; verified with the sender's public key
- [ ] Signed and verified with the same symmetric key
- [ ] Signed with the CA's private key; verified with the sender's public key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Signed with the sender's private key; verified with the sender's public key</p>
<p>Digital signatures prove integrity (message wasn't changed), authentication (proves the source), and non-repudiation. Any change to the message invalidates the signature.</p>
</details>

---

### 18. In blockchain technology, what happens if someone tries to alter data in an existing block?
- [ ] Nothing — blocks can be freely edited by any node
- [ ] The block's hash (and all following hashes) must be recalculated, and the altered chain no longer matches the rest of the network, so it's rejected
- [ ] The transaction is automatically re-verified and accepted
- [ ] Only the Certificate Authority can detect the change

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The block's hash (and all following hashes) must be recalculated, and the altered chain no longer matches the rest of the network, so it's rejected</p>
<p>Each block's hash is calculated from the previous blocks' data. Altering a block breaks that chain of hashes, so the altered version no longer matches what the rest of the network has stored and is rejected.</p>
</details>

---

### 19. What is a "Root of Trust" in the context of PKI?
- [ ] A wildcard certificate covering all subdomains
- [ ] An inherently trusted component (hardware, software, or firmware) that a third party vouches for, such as an HSM, secure enclave, or CA
- [ ] A password-protected TPM used for a single device
- [ ] A list of revoked certificates

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An inherently trusted component (hardware, software, or firmware) that a third party vouches for, such as an HSM, secure enclave, or CA</p>
<p>A Root of Trust builds trust from something otherwise unknown by having a trusted 3rd party vouch for it — examples include an HSM, secure enclave, or certificate authority.</p>
</details>

---

### 20. A certificate covering `*.birdfeeder.live` so it can be used across many subdomains is an example of what, also known as a Subject Alternative Name (SAN)?
- [ ] A self-signed certificate
- [ ] A wildcard certificate
- [ ] A certificate revocation list
- [ ] An OCSP staple

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A wildcard certificate</p>
<p>Wildcard certificates (an X.509 extension also known as Subject Alternative Name/SAN) allow one certificate to support many different domains under an organization.</p>
</details>

---

### 21. How does OCSP stapling improve on checking a traditional Certificate Revocation List (CRL)?
- [ ] It requires downloading the entire CRL file from the CA every time
- [ ] The cert holder verifies and provides its own signed status, stapled directly into the SSL/TLS handshake, avoiding a full list download
- [ ] It removes the need for a Certificate Authority entirely
- [ ] It only works with self-signed certificates

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The cert holder verifies and provides its own signed status, stapled directly into the SSL/TLS handshake, avoiding a full list download</p>
<p>OCSP stapling provides scalability: the cert holder's server stores and provides its own OCSP status, which is digitally signed by the CA and "stapled" into the TLS handshake — better than downloading an entire CRL.</p>
</details>
