# Quiz 1.2 — The CIA Triad
*Professor Messer SY0-701 · Section 1.2*

---

### 1. Which part of the CIA Triad is focused on preventing disclosure of information to unauthorized individuals or systems?
- [ ] Integrity
- [ ] Availability
- [ ] Confidentiality
- [ ] Non-repudiation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Confidentiality</p>
<p>Confidentiality prevents disclosure of information to unauthorized individuals or systems, using tools like encryption, access controls, and 2FA.</p>
</details>

---

### 2. Which principle ensures that messages can't be modified without detection, and that data is stored and transferred as intended?
- [ ] Confidentiality
- [ ] Integrity
- [ ] Availability
- [ ] Accounting

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Integrity</p>
<p>Integrity ensures data isn't modified without detection, using hashing, digital signatures, and certificates.</p>
</details>

---

### 3. Which of the following supports Availability in the CIA Triad?
- [ ] Redundancy and fault tolerance
- [ ] Hashing
- [ ] Access controls
- [ ] Digital signatures

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Redundancy and fault tolerance</p>
<p>Availability means systems and networks must be up and running, supported by redundancy, fault tolerance, and patching.</p>
</details>

---

### 4. A hash, also known as a message digest or fingerprint, provides proof of what?
- [ ] Proof of origin
- [ ] Proof of integrity
- [ ] Proof of authorization
- [ ] Proof of confidentiality

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Proof of integrity</p>
<p>A hash provides proof of integrity: it verifies data hasn't changed, but it doesn't associate the data with an individual.</p>
</details>

---

### 5. To prove the source of a message (proof of origin), the sender encrypts the hash of the message with which key?
- [ ] The receiver's public key
- [ ] The sender's public key
- [ ] The sender's private key
- [ ] A shared symmetric key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The sender's private key</p>
<p>The sender encrypts the hash with their private key; the receiver decrypts it with the sender's public key to confirm origin and non-repudiation.</p>
</details>

---

### 6. In the AAA framework, which step determines what access a user has based on their identity and authentication?
- [ ] Identification
- [ ] Authentication
- [ ] Authorization
- [ ] Accounting

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Authorization</p>
<p>Authorization determines what access you have based on your identification and authentication.</p>
</details>

---

### 7. Which AAA step records details like login time, data sent/received, and logout time?
- [ ] Accounting
- [ ] Identification
- [ ] Authorization
- [ ] Authentication

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Accounting</p>
<p>Accounting tracks login time, data sent/received, and logout time.</p>
</details>

---

### 8. Since a device can't type a password, how is a system typically authenticated?
- [ ] With a shared username/password
- [ ] With a digitally signed certificate
- [ ] With a physical access badge
- [ ] With a security question

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> With a digitally signed certificate</p>
<p>A device is authenticated by placing a digitally signed certificate on it, issued and validated by a trusted Certificate Authority (CA).</p>
</details>

---

### 9. What is a Gap Analysis primarily used to identify?
- [ ] The difference between the current state and a desired security baseline
- [ ] The list of all firewall rules
- [ ] The uptime of a system
- [ ] The encryption algorithm in use

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The difference between the current state and a desired security baseline</p>
<p>A Gap Analysis compares where an organization is against where it wants to be, working toward a known baseline like NIST or ISO/IEC.</p>
</details>

---

### 10. In the Zero Trust model, which component acts as the "gatekeeper" that can allow, monitor, and terminate connections?
- [ ] Policy Engine
- [ ] Policy Administrator
- [ ] Policy Enforcement Point (PEP)
- [ ] Policy Decision Point

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Policy Enforcement Point (PEP)</p>
<p>The PEP is the gatekeeper and can consist of multiple devices working together to allow, monitor, or terminate connections.</p>
</details>

---

### 11. Which Zero Trust plane is responsible for processing frames and packets, forwarding, encrypting, and NAT?
- [ ] Control Plane
- [ ] Data Plane
- [ ] Management Plane
- [ ] Application Plane

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data Plane</p>
<p>The Data Plane processes the actual network data: forwarding, encrypting, and NAT. The Control Plane manages policies and rules for the data plane.</p>
</details>

---

### 12. An access control vestibule is an example of which type of security control?
- [ ] Technical
- [ ] Physical
- [ ] Managerial
- [ ] Compensating

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Physical</p>
<p>Access control vestibules are a physical security control that promotes managed access through an area, one person or group at a time.</p>
</details>

---

### 13. What is the purpose of a honeypot?
- [ ] To encrypt sensitive files
- [ ] To create a virtual decoy environment that attracts and traps attackers
- [ ] To back up critical data
- [ ] To authenticate remote devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To create a virtual decoy environment that attracts and traps attackers</p>
<p>A honeypot creates a virtual world to attract attackers (usually automated) and trap them there, away from real systems.</p>
</details>

---

### 14. Fake API credentials or fake email addresses used to track malicious actors are known as what?
- [ ] Honeyfiles
- [ ] Honeynets
- [ ] Honeytokens
- [ ] Honeypots

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Honeytokens</p>
<p>Honeytokens are traceable fake data, like API credentials or email addresses, used to alert on or track malicious actors when used.</p>
</details>
