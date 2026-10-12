# Quiz 3.3 — Data Types and Classifications
*Professor Messer SY0-701 · Section 3.3*

---

### 1. Credit card data governed by government laws and statutes is an example of which data type?
- [ ] Trade secret
- [ ] Regulated
- [ ] Intellectual property
- [ ] Public

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Regulated</p>
<p>Regulated data is governed by government laws and statutes and may be managed by a third party.</p>
</details>

---

### 2. What is the difference between a trade secret and intellectual property?
- [ ] A trade secret is an organization's secret (like a formula); intellectual property may be publicly visible and is protected by copyright and trademark laws
- [ ] Intellectual property is always secret; trade secrets are always public
- [ ] They're the same thing
- [ ] Trade secrets are protected by copyright law

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A trade secret is an organization's secret (like a formula); intellectual property may be publicly visible and is protected by copyright and trademark laws</p>
<p>Trade secrets stay hidden, while intellectual property can be public but is legally protected.</p>
</details>

---

### 3. Which data type includes court records, documents, and judge/attorney info, often stored in many different systems?
- [ ] Financial information
- [ ] Legal information
- [ ] Trade secret
- [ ] Non-human readable

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Legal information</p>
<p>In legal information, PII and other details may be masked.</p>
</details>

---

### 4. Payment records and bank records fall under which data type?
- [ ] Legal information
- [ ] Financial information
- [ ] Intellectual property
- [ ] PHI

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Financial information</p>
<p>Financial information includes customer and company financials, payment records, and bank records.</p>
</details>

---

### 5. CSV, XML, and JSON are examples of which data format?
- [ ] Human-readable only
- [ ] Non-human readable only
- [ ] Hybrid
- [ ] Encrypted

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Hybrid</p>
<p>Data can be human-readable, non-human readable (like barcodes), or a hybrid that both people and machines can read, such as CSV, XML, and JSON.</p>
</details>

---

### 6. How might an organization protect health records differently than license tag numbers?
- [ ] Treat them exactly the same
- [ ] Add extra permissions, a different process to view the data, or restrict network access to the data source
- [ ] Make health records public
- [ ] Delete health records after viewing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Add extra permissions, a different process to view the data, or restrict network access to the data source</p>
<p>Health records are much more sensitive than license tag numbers, so classifying sensitive data lets you apply stronger controls where needed.</p>
</details>

---

### 7. Data that is the property of an organization, often unique to it and possibly including trade secrets, is called what?
- [ ] Public
- [ ] Proprietary
- [ ] Regulated
- [ ] Critical

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Proprietary</p>
<p>Proprietary data belongs to the organization and is often unique to it.</p>
</details>

---

### 8. What is the difference between PII and PHI?
- [ ] PII is data that can identify an individual; PHI is Protected Health Information associated with an individual, like health status, records, and payments
- [ ] PHI is any data that identifies a person; PII is only health data
- [ ] They're the same
- [ ] PII only applies to companies

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> PII is data that can identify an individual; PHI is Protected Health Information associated with an individual, like health status, records, and payments</p>
<p>Both are sensitive classifications, but PHI specifically covers health-related info.</p>
</details>

---

### 9. Which data classification describes data that is very sensitive and must be approved to view?
- [ ] Public
- [ ] Confidential
- [ ] Critical
- [ ] Sensitive

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Confidential</p>
<p>The classifications are: sensitive (IP, PII, PHI), confidential (very sensitive, approval needed), public (no restrictions), private/classified (may require an NDA), and critical (should always be accessible).</p>
</details>

---

### 10. Which data classification describes data that should always be accessible?
- [ ] Confidential
- [ ] Private
- [ ] Critical
- [ ] Public

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Critical</p>
<p>Critical data must always be available.</p>
</details>

---

### 11. Which data classification may require signing an NDA?
- [ ] Public
- [ ] Private / Classified
- [ ] Critical
- [ ] Hybrid

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Private / Classified</p>
<p>Private or classified data may require a non-disclosure agreement before you can access it.</p>
</details>

---

### 12. How is data at rest typically protected?
- [ ] With transport encryption like TLS
- [ ] By encrypting it (whole disk, database, or file/folder level) and applying permissions
- [ ] It can't be protected
- [ ] By keeping it only in RAM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By encrypting it (whole disk, database, or file/folder level) and applying permissions</p>
<p>Data at rest is data sitting on a storage device.</p>
</details>

---

### 13. Data being transmitted over the network is called what, and how is it protected?
- [ ] Data at rest; protected with disk encryption
- [ ] Data in transit (data in motion); protected with network-based protection like firewalls/IPS and transport encryption like TLS or IPsec
- [ ] Data in use; protected by keeping it in RAM
- [ ] Data sovereignty; protected by GDPR

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data in transit (data in motion); protected with network-based protection like firewalls/IPS and transport encryption like TLS or IPsec</p>
<p>Data in transit doesn't have much protection on its own while it travels.</p>
</details>

---

### 14. Why is data in use especially vulnerable?
- [ ] It's always stored on removable drives
- [ ] It's actively processing in memory (RAM, CPU, cache, registers) and is almost always in decrypted form, so attackers can pick it out of RAM
- [ ] It's always sent over unencrypted networks
- [ ] It's never accessed by applications

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's actively processing in memory (RAM, CPU, cache, registers) and is almost always in decrypted form, so attackers can pick it out of RAM</p>
<p>Data has to be decrypted to be processed, which makes memory an attractive target.</p>
</details>

---

### 15. What is data sovereignty?
- [ ] The idea that data residing in a country is subject to the laws of that country
- [ ] A type of encryption algorithm
- [ ] The right of any company to store data anywhere
- [ ] A method of hashing data

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The idea that data residing in a country is subject to the laws of that country</p>
<p>This applies to legal proceedings and court orders, and laws may restrict where data can be stored. For example, under the EU's GDPR, data collected on EU citizens must be stored in the EU.</p>
</details>

---

### 16. How can geolocation be used to protect data?
- [ ] By encrypting data in RAM
- [ ] By managing data access based on location, like preventing access from other countries or limiting admin tasks unless a secure area is used
- [ ] By replacing data with tokens
- [ ] By hashing all location data

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By managing data access based on location, like preventing access from other countries or limiting admin tasks unless a secure area is used</p>
<p>Geolocation uses 802.11 info, GPS info, and mobile provider info to determine location details.</p>
</details>

---

### 17. What is geofencing?
- [ ] Building a physical fence around a data center
- [ ] Automatically allowing or restricting access when a user is in a particular location
- [ ] Encrypting data by country
- [ ] Storing data only in the EU

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Automatically allowing or restricting access when a user is in a particular location</p>
<p>Geographic restrictions can be based on network location (IP subnet, which is difficult with mobile networks) or geolocation (GPS is best for mobile, plus 802.11/IP).</p>
</details>

---

### 18. In encryption, what does "confusion" mean?
- [ ] The encrypted data is drastically different from the plaintext
- [ ] The data can never be decrypted
- [ ] The key is lost
- [ ] Two inputs produce the same output

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The encrypted data is drastically different from the plaintext</p>
<p>Encryption turns plaintext into unreadable ciphertext. It's a two-way street, since decryption is possible with the right key.</p>
</details>

---

### 19. How is hashing different from encryption?
- [ ] Hashing is a one-way trip that represents data as a short fingerprint/digest, while encryption can be decrypted with the right key
- [ ] Hashing can always be reversed with a key
- [ ] Encryption is a one-way trip
- [ ] They're identical

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Hashing is a one-way trip that represents data as a short fingerprint/digest, while encryption can be decrypted with the right key</p>
<p>Hashing verifies integrity (e.g. a downloaded document matches the original) and can be used in digital signatures for authentication, non-repudiation, and integrity.</p>
</details>

---

### 20. Turning perfectly readable code into nonsense to protect a codebase is an example of what?
- [ ] Tokenization
- [ ] Obfuscation
- [ ] Segmentation
- [ ] Hashing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Obfuscation</p>
<p>Obfuscation makes something normally understandable very difficult to understand. It can also be used in malicious code.</p>
</details>

---

### 21. Which data protection technique hides some of the original data, possibly only from view while it's still stored normally?
- [ ] Data masking
- [ ] Tokenization
- [ ] Encryption
- [ ] Geofencing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data masking</p>
<p>Data masking protects PII and other sensitive data using techniques like substituting, shuffling, encrypting, and masking out.</p>
</details>

---

### 22. Why is tokenization useful in credit card processing?
- [ ] It encrypts the card number with a strong key
- [ ] It replaces the card number with a non-sensitive placeholder, so an attacker who captures it can't use it later
- [ ] It hashes the card number
- [ ] It stores the card number in plaintext

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It replaces the card number with a non-sensitive placeholder, so an attacker who captures it can't use it later</p>
<p>Tokenization is not encryption or hashing — it simply substitutes a placeholder for the sensitive data.</p>
</details>

---

### 23. Why is data segmentation better than using a single data source?
- [ ] It makes all data public
- [ ] Separating data into smaller pieces in different locations lets sensitive data get stronger security
- [ ] It removes the need for permissions
- [ ] It's required by GDPR for all data

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Separating data into smaller pieces in different locations lets sensitive data get stronger security</p>
<p>Many organizations use a single data source, which is bad. Segmentation lets you apply stronger security to the most sensitive data, along with permission restrictions.</p>
</details>
