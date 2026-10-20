# Quiz 4.3 — Vulnerability Scanning
*Professor Messer SY0-701 · Section 4.3*

---

### 1. Which of the following describes vulnerability scanning?
- [ ] It's highly invasive and always exploits systems
- [ ] It's usually minimally invasive, tests from both the outside and inside, and gathers as much info as possible
- [ ] It only tests from outside the network
- [ ] It never produces reports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's usually minimally invasive, tests from both the outside and inside, and gathers as much info as possible</p>
<p>Scans include port scans to see what's open for an attack, and scanner engines are good at identifying systems and security devices. You then have to sift through the reports afterward.</p>
</details>

---

### 2. Why can't you rely entirely on Static Application Security Testing (SAST)?
- [ ] It can't find any flaws in code
- [ ] Not everything can be found through analysis (like authentication security or insecure cryptography), and false positives mean each finding must be verified
- [ ] It only works on running applications
- [ ] It requires physical access to the server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Not everything can be found through analysis (like authentication security or insecure cryptography), and false positives mean each finding must be verified</p>
<p>SAST helps identify security flaws in code, but don't rely on automation for everything.</p>
</details>

---

### 3. What is fuzzing?
- [ ] Reviewing source code line by line
- [ ] Dynamic analysis that sends random input to an application, looking for crashes, server errors, or exceptions
- [ ] Encrypting application input
- [ ] Scanning for open ports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Dynamic analysis that sends random input to an application, looking for crashes, server errors, or exceptions</p>
<p>Fuzzing is also called fault-injecting, robustness testing, syntax testing, or negative testing. It shows where input validation is needed.</p>
</details>

---

### 4. What is a drawback of fuzzing engines?
- [ ] They only run once
- [ ] They're very time and processor intensive, needing many iterations to test an app
- [ ] They can't find any errors
- [ ] There's only one fuzzing engine available

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They're very time and processor intensive, needing many iterations to test an app</p>
<p>There are many different fuzzing engine options.</p>
</details>

---

### 5. What should you confirm when monitoring an application package?
- [ ] That it's the largest version available
- [ ] That it comes from a trusted source with no added malware or embedded vulnerabilities, testing it in a lab before deployment
- [ ] That it was downloaded the fastest
- [ ] That it has no documentation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> That it comes from a trusted source with no added malware or embedded vulnerabilities, testing it in a lab before deployment</p>
<p>Some apps are distributed in a package, so confirm the package is legitimate before deploying it.</p>
</details>

---

### 6. What does OSINT stand for, and what does it use?
- [ ] Open-Source Intelligence — publicly available sources like discussion groups, social media, government data, and commercial data
- [ ] Operational Security Intelligence — classified military data
- [ ] Offline System Intelligence — internal logs only
- [ ] Open Server Integration — cloud APIs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Open-Source Intelligence — publicly available sources like discussion groups, social media, government data, and commercial data</p>
<p>Government data includes public hearings, reports, and websites. Commercial data includes maps, financial reports, and databases.</p>
</details>

---

### 7. What can third-party threat intelligence provide?
- [ ] Only a list of passwords
- [ ] Threat info someone else has already compiled, plus services like threat analysis, correlation across data sources, and constant monitoring for automated threat prevention
- [ ] Physical security guards
- [ ] A replacement for patching

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Threat info someone else has already compiled, plus services like threat analysis, correlation across data sources, and constant monitoring for automated threat prevention</p>
<p>Threat intelligence covers researching threats and threat actors, such as hacker group profiles and the tools attackers use.</p>
</details>

---

### 8. How does the Cyber Threat Alliance (CTA) work?
- [ ] Members upload formatted threat intelligence, the CTA scores and validates each submission, and other members can extract the validated data
- [ ] It sells stolen credit cards
- [ ] It only shares classified government info
- [ ] It runs penetration tests for members

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Members upload formatted threat intelligence, the CTA scores and validates each submission, and other members can extract the validated data</p>
<p>Organizations need to share critical security details. Public threat intelligence is often classified, while private companies have extensive resources.</p>
</details>

---

### 9. What is the dark web, and why is it useful for threat intelligence?
- [ ] A public search engine
- [ ] Overlay networks on the internet that need specific software to access, where hacking groups sell credit cards, tools, techniques, and account credentials
- [ ] A government database of vulnerabilities
- [ ] A type of VPN

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Overlay networks on the internet that need specific software to access, where hacking groups sell credit cards, tools, techniques, and account credentials</p>
<p>Monitoring the dark web can reveal what attackers are selling or planning.</p>
</details>

---

### 10. How does penetration testing differ from vulnerability scanning?
- [ ] Pentesting performs actual exploits to simulate an attack on your own systems
- [ ] Pentesting is less invasive
- [ ] Pentesting never touches live systems
- [ ] They're exactly the same

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Pentesting performs actual exploits to simulate an attack on your own systems</p>
<p>Pentesting is often a compliance mandate, with regular testing done by a third party.</p>
</details>

---

### 11. What does a pentest's rules of engagement document define?
- [ ] Only the price of the test
- [ ] The purpose and scope, testing type and schedule, IP address ranges, emergency contacts, sensitive info handling, and in-scope vs. out-of-scope devices
- [ ] The attacker's real identity
- [ ] The company's firewall passwords

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The purpose and scope, testing type and schedule, IP address ranges, emergency contacts, sensitive info handling, and in-scope vs. out-of-scope devices</p>
<p>Testing types include on-site physical breaches and internal or external tests, and the schedule might be normal working hours or after 6pm only.</p>
</details>

---

### 12. Why must pentesters be careful when exploiting vulnerabilities?
- [ ] Exploits can cause a denial of service or loss of data, and buffer overflows can cause instability
- [ ] Exploits are always harmless
- [ ] They might accidentally patch the system
- [ ] Exploits only work on test systems

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Exploits can cause a denial of service or loss of data, and buffer overflows can cause instability</p>
<p>Testers may try many vulnerability types (social engineering, brute force, database injections), and you're only sure you're vulnerable if security can actually be bypassed.</p>
</details>

---

### 13. In the pentest process, what is lateral movement?
- [ ] Getting into the network for the first time
- [ ] Moving from system to system inside the network, which is often less protected
- [ ] Setting up a backdoor to get back in
- [ ] Writing the final report

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Moving from system to system inside the network, which is often less protected</p>
<p>The process goes: initial exploitation (get in), lateral movement, persistence (ensure a way back in), and the pivot.</p>
</details>

---

### 14. In the pentest process, what is persistence?
- [ ] Trying the same password repeatedly
- [ ] Making sure there's a way back in, such as setting up a backdoor or changing passwords
- [ ] Using a system as a relay to reach other systems
- [ ] Scanning ports continuously

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Making sure there's a way back in, such as setting up a backdoor or changing passwords</p>
<p>Once you're in, persistence keeps your access.</p>
</details>

---

### 15. What is "the pivot" in penetration testing?
- [ ] Turning off the firewall
- [ ] Using a vulnerable system as a proxy or relay to reach systems that normally aren't accessible
- [ ] Reporting the vulnerability to the vendor
- [ ] Rebooting a compromised server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Using a vulnerable system as a proxy or relay to reach systems that normally aren't accessible</p>
<p>A compromised system becomes a stepping stone deeper into the network.</p>
</details>

---

### 16. What is a bug bounty program?
- [ ] A fine for writing buggy code
- [ ] A reward for discovering and documenting vulnerabilities, as part of a responsible disclosure program
- [ ] A type of malware
- [ ] An insurance policy

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A reward for discovering and documenting vulnerabilities, as part of a responsible disclosure program</p>
<p>Fixing a vulnerability takes time (software changes, testing, deployment), so responsible disclosure releases the info in a controlled way after the fix is applied.</p>
</details>

---

### 17. What is a false positive in vulnerability scanning?
- [ ] A real vulnerability that wasn't detected
- [ ] A vulnerability that's identified but doesn't actually exist
- [ ] A low-severity vulnerability
- [ ] A vulnerability that has already been patched and verified

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A vulnerability that's identified but doesn't actually exist</p>
<p>This is different from a low-severity vulnerability, which is real but may not be your highest priority.</p>
</details>

---

### 18. What is a false negative?
- [ ] A vulnerability exists, but you didn't detect it
- [ ] A vulnerability is detected but doesn't exist
- [ ] A vulnerability with a CVSS score of 0
- [ ] A patched vulnerability

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A vulnerability exists, but you didn't detect it</p>
<p>To minimize false information, update to the latest signatures and work with the vulnerability detection manufacturer.</p>
</details>

---

### 19. How should you prioritize vulnerabilities when it's hard to tell how severe they are?
- [ ] Treat every vulnerability as critical
- [ ] Refer to public disclosures and vulnerability databases, since the research has probably already been done
- [ ] Ignore informational findings entirely without review
- [ ] Fix them in alphabetical order

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Refer to public disclosures and vulnerability databases, since the research has probably already been done</p>
<p>Not every vulnerability shares the same priority — some may not be significant, others are critical, and some are informational.</p>
</details>

---

### 20. What is CVSS, and how is it scored?
- [ ] Common Vulnerability Scoring System — scores vulnerabilities from 0 to 10, with 10 being most critical
- [ ] Common Vulnerabilities and Exposures — a list of vulnerability IDs
- [ ] Cyber Vulnerability Security Standard — scored A through F
- [ ] Central Vulnerability Scanning Service — scored 1 to 100

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Common Vulnerability Scoring System — scores vulnerabilities from 0 to 10, with 10 being most critical</p>
<p>CVSS scores are found in the National Vulnerability Database (nvd.nist.gov). Scoring standards change over time, and CVSS 2.0 scores differently than CVSS 3.x.</p>
</details>

---

### 21. What is the CVE database used for?
- [ ] Scoring vulnerabilities from 0 to 10
- [ ] Cross-referencing vulnerabilities online, since almost all scanners point you to it
- [ ] Storing cybersecurity insurance claims
- [ ] Hosting bug bounty payments

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Cross-referencing vulnerabilities online, since almost all scanners point you to it</p>
<p>The Common Vulnerabilities and Exposures (CVE) database is at cve.mitre.org, and Microsoft Security Bulletins are another reference. Some vulnerabilities can't be definitively identified by a scanner and must be checked manually.</p>
</details>

---

### 22. A scan looking for misconfigured firewalls, open ports, and vulnerable devices is which type of scan?
- [ ] Application scan
- [ ] Web application scan
- [ ] Network scan
- [ ] Static code scan

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network scan</p>
<p>Application scans cover desktop and mobile apps, and web application scans cover software on a web server.</p>
</details>

---

### 23. What is exposure factor?
- [ ] The number of users on a system
- [ ] The loss of value or business activity if a vulnerability is exploited, usually expressed as a percentage
- [ ] The CVSS score of a vulnerability
- [ ] The time it takes to patch

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The loss of value or business activity if a vulnerability is exploited, usually expressed as a percentage</p>
<p>For example, a small DDoS that limits access to a service might get a 50% exposure factor, while a buffer overflow that fully disables a service gets 100%. It's a consideration when prioritizing fixes.</p>
</details>

---

### 24. Why do environmental variables matter when prioritizing vulnerabilities?
- [ ] All environments are identical
- [ ] Environments differ in number and type of users, revenue generation, and potential for exploit — a device in an isolated test lab has different priority than a database server in the public cloud
- [ ] They only affect the CVSS score
- [ ] Environmental variables only apply to physical security

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Environments differ in number and type of users, revenue generation, and potential for exploit — a device in an isolated test lab has different priority than a database server in the public cloud</p>
<p>The environment affects both prioritization and patching frequency.</p>
</details>

---

### 25. What happened at Tallahassee Memorial HealthCare in February 2023?
- [ ] A bug bounty paid out a record amount
- [ ] Ransomware brought down surgeries for two weeks
- [ ] A false positive shut down the network
- [ ] A pentest accidentally deleted patient records

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Ransomware brought down surgeries for two weeks</p>
<p>This is an example of industry/organizational impact, where some exploits have significant consequences. Power utilities are another high-impact example.</p>
</details>

---

### 26. Why does risk tolerance affect the timing of security patches?
- [ ] Patching immediately skips proper testing, but testing takes time and you're vulnerable during that period
- [ ] Patches should never be tested
- [ ] Organizations can always remove all risk
- [ ] Risk tolerance only applies to insurance

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Patching immediately skips proper testing, but testing takes time and you're vulnerable during that period</p>
<p>Risk tolerance is the amount of risk acceptable to an organization, since it's impractical to remove all risk.</p>
</details>

---

### 27. Which of these does cybersecurity insurance typically NOT cover?
- [ ] Lost revenue
- [ ] Data recovery costs
- [ ] Privacy lawsuit costs
- [ ] Intentional acts and fund transfers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Intentional acts and fund transfers</p>
<p>Cybersecurity insurance can cover lost revenue, data recovery costs, money lost to phishing, and privacy lawsuit costs. Ransomware has increased its popularity.</p>
</details>

---

### 28. What is the most common vulnerability mitigation technique?
- [ ] Buying insurance
- [ ] Patching
- [ ] Air gapping every device
- [ ] Ignoring low-severity findings

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Patching</p>
<p>Patching is an ongoing process — you have a patch file to install for a vulnerability you know exists.</p>
</details>

---

### 29. How does segmentation help with vulnerability remediation?
- [ ] It patches the vulnerability automatically
- [ ] It limits the scope of an exploit by separating devices into their own networks/VLANs, and internal NGFWs can block unwanted traffic between VLANs
- [ ] It removes the need for firewalls
- [ ] It makes all devices publicly accessible

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It limits the scope of an exploit by separating devices into their own networks/VLANs, and internal NGFWs can block unwanted traffic between VLANs</p>
<p>If a device can't be patched, you can disconnect it from the world with an air gap.</p>
</details>

---

### 30. What is needed for devices on different VLANs to communicate?
- [ ] Nothing, since VLANs always share traffic
- [ ] A layer 3 device
- [ ] A degausser
- [ ] A certificate of destruction

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A layer 3 device</p>
<p>VLANs are logically separated instead of physically separated (which uses multiple units and separate infrastructure).</p>
</details>

---

### 31. If a patch can't be deployed, which of these is a compensating control?
- [ ] Doing nothing until the next year
- [ ] Disabling the problematic service, revoking access to the app, limiting external access, or modifying internal security controls and software firewalls
- [ ] Publishing the vulnerability online
- [ ] Removing all firewalls

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Disabling the problematic service, revoking access to the app, limiting external access, or modifying internal security controls and software firewalls</p>
<p>Compensating controls provide coverage until a patch is deployed. Revoking access to the app affects all users, too.</p>
</details>

---

### 32. When is an exception or exemption an option for a vulnerability?
- [ ] Whenever a team doesn't want to patch
- [ ] When something can't be patched, usually through a formal approval process that balances providing the service with protecting data and systems
- [ ] Only for critical vulnerabilities
- [ ] Never

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> When something can't be patched, usually through a formal approval process that balances providing the service with protecting data and systems</p>
<p>Not all vulnerabilities share the same severity — some may require a local login, physical access, or other criteria to exploit.</p>
</details>

---

### 33. How do you validate that remediation actually worked?
- [ ] Assume the patch worked
- [ ] Rescanning, auditing remediated systems to ensure the patch deployed, and manually verifying the system's security
- [ ] Wait for an attacker to try again
- [ ] Delete the vulnerability report

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Rescanning, auditing remediated systems to ensure the patch deployed, and manually verifying the system's security</p>
<p>Once a vulnerability is patched, you still need to confirm the patch actually stopped the exploit.</p>
</details>

---

### 34. Why is continuous vulnerability reporting needed?
- [ ] Vulnerabilities only appear once
- [ ] New vulnerabilities are continuously discovered, so ongoing reports track identified vulnerabilities, patched vs. unpatched systems, new threats, and errors, exceptions, and exemptions
- [ ] Reports replace the need for scanning
- [ ] It's only required for insurance

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> New vulnerabilities are continuously discovered, so ongoing reports track identified vulnerabilities, patched vs. unpatched systems, new threats, and errors, exceptions, and exemptions</p>
<p>Ongoing checks are difficult to manage without automation.</p>
</details>
