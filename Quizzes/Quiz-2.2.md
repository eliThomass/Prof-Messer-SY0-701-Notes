# Quiz 2.2 — Common Threat Vectors
*Professor Messer SY0-701 · Section 2.2*

---

### 1. What is a threat vector?
- [ ] A list of revoked certificates
- [ ] A method used by an attacker to gain access to a target
- [ ] A category of threat actor motivation
- [ ] A type of encryption algorithm

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A method used by an attacker to gain access to a target</p>
<p>A threat vector is a method used by the attacker to gain access to the target — IT security professionals spend their careers watching these vectors.</p>
</details>

---

### 2. Which category is described as one of the biggest and most successful threat vectors, including email and SMS-based attacks?
- [ ] File-based vectors
- [ ] Message-based vectors
- [ ] Voice call vectors
- [ ] Image-based vectors

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Message-based vectors</p>
<p>Message-based vectors are one of the biggest and most successful threat vectors, including email with malicious links/downloads, SMS, phishing, and social engineering attacks like invoice or crypto scams.</p>
</details>

---

### 3. Why is the SVG image format considered a security concern as a threat vector?
- [ ] It can only be opened by specialized software
- [ ] It's described in XML, which can allow HTML injection and JavaScript attack code
- [ ] It always contains an embedded virus
- [ ] It requires macros to render

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's described in XML, which can allow HTML injection and JavaScript attack code</p>
<p>Because SVG images are described in XML, they raise significant security concerns like HTML injection and JavaScript attack code, so browsers must provide input validation.</p>
</details>

---

### 4. Which of these is an example of a file-based threat vector?
- [ ] A Bluetooth reconnaissance scan
- [ ] A Microsoft Office document containing macros
- [ ] An open TCP port
- [ ] A war dialing scan

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A Microsoft Office document containing macros</p>
<p>File-based vectors go beyond just .exe files — they include Adobe PDFs (which can contain other embedded objects), compressed files with many files inside, and Microsoft Office documents with macros or add-ins.</p>
</details>

---

### 5. What is "vishing"?
- [ ] Phishing conducted over a phone call
- [ ] Phishing conducted via SMS text message
- [ ] A URL hijacking technique using a replaced letter
- [ ] Lying to a victim while playing a fictional character

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Phishing conducted over a phone call</p>
<p>Vishing is phishing over the phone — a classic voice call vector.</p>
</details>

---

### 6. What is "war dialing"?
- [ ] Sending spam over IP-based phone systems at large scale
- [ ] Attackers trying to find unpublished phone numbers they can use to gain access to systems
- [ ] Tampering with a phone call in progress
- [ ] Dropping infected USB drives in a parking lot

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Attackers trying to find unpublished phone numbers they can use to gain access to systems</p>
<p>War dialing is when attackers try to find unpublished phone numbers that they can use to gain access to systems, distinct from spam over IP or call tampering.</p>
</details>

---

### 7. Leaving infected USB flash drives in a company parking lot is an example of which threat vector, and why is it effective against air-gapped networks?
- [ ] Removable device vectors — it can infect air-gapped networks with little effort and no bandwidth
- [ ] Supply chain vectors — it compromises the manufacturing process
- [ ] Unsecure network vectors — it exploits open wireless networks
- [ ] Voice call vectors — it relies on social engineering over the phone

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Removable device vectors — it can infect air-gapped networks with little effort and no bandwidth</p>
<p>Removable device vectors get around the firewall entirely with USB devices, can infect air-gapped networks, and allow data exfiltration with little effort and no bandwidth.</p>
</details>

---

### 8. In "agentless" vulnerable software vectors, why can a compromised application on a server affect all users?
- [ ] Because each client installs its own local .exe file
- [ ] Because the client runs a new instance from the server each time, with no installed executable
- [ ] Because agentless software cannot be patched
- [ ] Because agentless software only runs on removable devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Because the client runs a new instance from the server each time, with no installed executable</p>
<p>Agentless vectors have no installed .exe — the client runs a new instance each time, so compromised software on the server would affect all users, unlike client-based vectors with locally installed executables.</p>
</details>

---

### 9. What is the primary risk of "unsupported systems" as a threat vector?
- [ ] They are always more expensive to operate
- [ ] They aren't patched, sometimes with no option to patch them at all, and outdated systems may go unnoticed without a full inventory
- [ ] They require 802.1X authentication
- [ ] They can only be exploited through Bluetooth

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They aren't patched, sometimes with no option to patch them at all, and outdated systems may go unnoticed without a full inventory</p>
<p>Unsupported systems aren't patched (maybe with no option to patch), and a single outdated system could be an entry point — organizations should keep an inventory of all systems.</p>
</details>

---

### 10. Which unsecure network vector uses 802.1X to help secure the network interface itself?
- [ ] Wireless
- [ ] Wired
- [ ] Bluetooth
- [ ] Open service ports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Wired</p>
<p>Wired network vectors involve unsecure interfaces that need 802.1X for authentication, whereas wireless vectors deal with outdated security protocols and open/rogue networks, and Bluetooth is often used for reconnaissance into an organization.</p>
</details>

---

### 11. Why is every open network service port considered an opportunity for an attacker?
- [ ] Ports cannot be closed once opened
- [ ] Each open port could expose an app misconfiguration or vulnerability, and more services generally means more open ports and potentially less security
- [ ] Open ports always use UDP, which cannot be firewalled
- [ ] Open ports are only a risk on removable devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Each open port could expose an app misconfiguration or vulnerability, and more services generally means more open ports and potentially less security</p>
<p>Network services connect via UDP or TCP ports; every open port is an opportunity for an attacker due to possible app misconfiguration or vulnerability, so firewall rules matter.</p>
</details>

---

### 12. What is the simplest and most direct mitigation against the "default credentials" threat vector?
- [ ] Install an HSM
- [ ] Change the default password
- [ ] Enable OCSP stapling
- [ ] Use a wildcard certificate

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Change the default password</p>
<p>The default credentials vector is mitigated simply by changing default passwords on devices and services before deployment.</p>
</details>

---

### 13. In the 2013 Target breach example, how did attackers gain access to point-of-sale systems across the company?
- [ ] Through a supply chain compromise of a Managed Service Provider (MSP) with access to many customer networks
- [ ] Through a watering hole attack on a coffee shop website
- [ ] Through war dialing unpublished phone numbers
- [ ] Through a wildcard certificate compromise

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Through a supply chain compromise of a Managed Service Provider (MSP) with access to many customer networks</p>
<p>MSPs access many different customer networks from one location, making them a perfect target — compromising the MSP gave attackers access to systems, as happened with malware on Target's POS systems in 2013.</p>
</details>

---

### 14. Counterfeit Cisco switches or other fake networking equipment represent which type of threat vector?
- [ ] Supply chain vector
- [ ] File-based vector
- [ ] Image-based vector
- [ ] Message-based vector

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Supply chain vector</p>
<p>Supply chain vectors include tampering with underlying infrastructure or the manufacturing process, such as suppliers producing counterfeit networking equipment.</p>
</details>

---

### 15. How is phishing best described?
- [ ] Encrypting data before exfiltration
- [ ] Social engineering with a touch of spoofing, often delivered by email or text
- [ ] A method for testing backup and recovery procedures
- [ ] A hardware-based cryptographic attack

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Social engineering with a touch of spoofing, often delivered by email or text</p>
<p>Phishing is social engineering with a touch of spoofing — check the URL and website graphics carefully, since it's often delivered by email, text, etc.</p>
</details>

---

### 16. In Business Email Compromise (BEC), how do attackers typically exploit trust in work email addresses?
- [ ] By stealing hardware security modules
- [ ] By spoofing an email address that's very close to a real company address to commit financial fraud
- [ ] By exploiting open Bluetooth ports
- [ ] By war dialing company phone lines

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By spoofing an email address that's very close to a real company address to commit financial fraud</p>
<p>BEC exploits trust in work email — attackers use spoofed addresses very close to the real company's, sending emails with updated bank info or using password reset features to commit financial fraud.</p>
</details>

---

### 17. What is typo-squatting?
- [ ] A type of URL hijacking that relies on a commonly mistyped or replaced letter in a domain name
- [ ] Lying to a victim while pretending to be someone else
- [ ] Phishing conducted via SMS
- [ ] Extracting information using psychological techniques

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A type of URL hijacking that relies on a commonly mistyped or replaced letter in a domain name</p>
<p>Typo-squatting is a type of URL hijacking, such as registering a domain with one letter replaced from the legitimate site.</p>
</details>

---

### 18. What is "pretexting" in social engineering?
- [ ] Sending phishing messages via SMS
- [ ] Lying to get information while the attacker plays the role of a character
- [ ] Registering a look-alike domain name
- [ ] Leaving an infected USB drive in a parking lot

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Lying to get information while the attacker plays the role of a character</p>
<p>Pretexting involves lying to get information — the attacker sets up a story and plays a character to be convincing.</p>
</details>

---

### 19. What is "smishing"?
- [ ] Phishing conducted over a phone call
- [ ] Phishing conducted via SMS text message
- [ ] Impersonating a brand online
- [ ] A watering hole attack

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Phishing conducted via SMS text message</p>
<p>Smishing is SMS phishing, alongside vishing (voice phishing) as common phishing tricks.</p>
</details>

---

### 20. "Eliciting information" from a victim, often seen alongside vishing, relies on what?
- [ ] Simply asking the victim directly for their password
- [ ] Well-documented psychological techniques to extract info without directly demanding it
- [ ] Brute-forcing a login form
- [ ] Exploiting an open network port

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Well-documented psychological techniques to extract info without directly demanding it</p>
<p>Eliciting information is about extracting info from the victim using well-documented psychological techniques, often paired with vishing — not simply asking "what's your password."</p>
</details>

---

### 21. If an attacker commits bank fraud by gaining access to a victim's account, what fraud might they escalate to next using that access?
- [ ] Government benefits fraud only
- [ ] Loan fraud, since they can now use the compromised bank access to get a loan
- [ ] Watering hole attacks
- [ ] Typo-squatting

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Loan fraud, since they can now use the compromised bank access to get a loan</p>
<p>Identity fraud can escalate: once an attacker has bank fraud access, they can leverage that to commit loan fraud, in addition to credit card fraud or government benefits fraud (e.g. filing fraudulent tax forms to steal a refund).</p>
</details>

---

### 22. In a watering hole attack, why do attackers infect a third-party website like a local coffee shop's site instead of attacking the target directly?
- [ ] Because the target group's secure systems can't be accessed directly, so attackers wait for the group to come to a site they commonly visit
- [ ] Because coffee shop websites have no security at all
- [ ] Because it guarantees infecting only the intended target and no one else
- [ ] Because it bypasses the need for any malware

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Because the target group's secure systems can't be accessed directly, so attackers wait for the group to come to a site they commonly visit</p>
<p>In a watering hole attack, attackers can't get into a secure system directly, so they infect a third-party site the victim group commonly uses, infecting all visitors but focusing only on specific ones of interest.</p>
</details>

---

### 23. Which pair of defense-in-depth controls is described as working together against a watering hole attack, where one lets traffic through and the other inspects and blocks it?
- [ ] Firewall and IPS
- [ ] TPM and HSM
- [ ] CRL and OCSP
- [ ] VPN and 802.1X

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Firewall and IPS</p>
<p>Defense-in-depth uses multiple layers: a firewall might allow traffic through, but an IPS inspects the contents and can block malicious traffic, alongside up-to-date anti-virus/anti-malware signatures.</p>
</details>

---

### 24. What is the general process behind a misinformation campaign, as described in the notes?
- [ ] Post on social media -> amplify message -> create fake users -> create content
- [ ] Create fake users -> create content -> post on social media -> amplify message -> real users share -> mass media picks up the story
- [ ] Create content -> mass media picks up the story -> amplify message -> create fake users
- [ ] Amplify message -> create fake users -> post on social media -> create content

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Create fake users -> create content -> post on social media -> amplify message -> real users share -> mass media picks up the story</p>
<p>Misinformation campaigns disseminate factually incorrect info to create confusion and division, often via influence campaigns enabled through social media, following this general spread pattern.</p>
</details>

---

### 25. Why do attackers create thousands of brand-impersonation websites for a well-known company?
- [ ] To get indexed by search engines so victims find them via search, virtually guaranteeing malware infection
- [ ] To reduce the company's search engine ranking
- [ ] To avoid having to register any domain names
- [ ] To bypass the need for any social engineering

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To get indexed by search engines so victims find them via search, virtually guaranteeing malware infection</p>
<p>Brand impersonation involves pretending to be a well-known brand and creating thousands of impersonated sites to get into search engine indexes like Google, making malware infection almost guaranteed for victims who land on them.</p>
</details>
