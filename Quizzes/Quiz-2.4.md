# Quiz 2.4 — An Overview of Malware
*Professor Messer SY0-701 · Section 2.4*

---

### 1. What happens to your data in a typical ransomware attack, and what usually remains available?
- [ ] All files are deleted; the OS is also destroyed
- [ ] Malware encrypts your data files, while your OS remains available
- [ ] The OS is encrypted, but your files remain untouched
- [ ] Nothing is encrypted; you're just shown ads

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Malware encrypts your data files, while your OS remains available</p>
<p>Ransomware encrypts your data files while the OS remains available; you must pay a fee or do something to get a decryption key back. Protect yourself with offline backups, updated OS/apps, and updated anti-virus signatures.</p>
</details>

---

### 2. What is the key difference between a virus and a worm?
- [ ] A virus self-propagates over the network; a worm needs you to execute a program
- [ ] A virus needs you to execute a program to reproduce; a worm self-replicates without needing you to do anything
- [ ] Worms only infect boot sectors; viruses only infect memory
- [ ] There is no difference — they're the same threat

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A virus needs you to execute a program to reproduce; a worm self-replicates without needing you to do anything</p>
<p>A virus reproduces through file systems or the network but needs you to execute a program. A worm uses the network as a transmission medium and self-propagates and spreads quickly on its own.</p>
</details>

---

### 3. What makes a fileless virus especially hard to detect?
- [ ] It only infects Microsoft Office macros
- [ ] It operates in memory and is never installed as a file or app on disk
- [ ] It only spreads through USB drives
- [ ] It requires a boot sector infection first

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It operates in memory and is never installed as a file or app on disk</p>
<p>A fileless virus is a stealth attack that avoids anti-virus detection — e.g. a user clicks a malicious link, a Flash/Java/Windows vulnerability launches PowerShell, downloads a payload into RAM, and runs it entirely in memory, adding an auto-start registry entry to persist across reboots.</p>
</details>

---

### 4. Which well-known worm is mentioned as an example that firewalls and IPS can help mitigate?
- [ ] WannaCry
- [ ] Mirai
- [ ] Stuxnet
- [ ] Conficker

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> WannaCry</p>
<p>Worms self-propagate and spread quickly using the network as a transmission medium; firewalls and IPS can mitigate many worm infestations, like WannaCry.</p>
</details>

---

### 5. Why does removing spyware/adware often require more than just anti-virus software?
- [ ] Spyware always reinstalls itself from the cloud
- [ ] Cleaning adware isn't easy, so it's recommended to keep a backup and run additional scans (like Malwarebytes)
- [ ] Anti-virus software cannot detect any spyware at all
- [ ] Spyware only exists on mobile devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Cleaning adware isn't easy, so it's recommended to keep a backup and run additional scans (like Malwarebytes)</p>
<p>Spyware spies on you through ads, identity theft, affiliate fraud, browser monitoring, and keyloggers. Anti-virus usually protects against it, but cleaning adware isn't easy.</p>
</details>

---

### 6. Why does bloatware ship on new computers and phones in the first place?
- [ ] It's required by the operating system to function
- [ ] Manufacturers are usually paid to include these extra apps
- [ ] It's installed by the end user by accident
- [ ] It replaces the need for an antivirus

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Manufacturers are usually paid to include these extra apps</p>
<p>Bloatware is installed by the manufacturer, who is usually being paid to include it. It adds to overall resource usage, slows the system, and could leave it open to exploits.</p>
</details>

---

### 7. Why can keyloggers circumvent encryption protections?
- [ ] They intercept encrypted network traffic directly
- [ ] They capture keystrokes as you type them, before encryption is ever applied
- [ ] They decrypt files stored on disk
- [ ] They only work on unencrypted websites

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They capture keystrokes as you type them, before encryption is ever applied</p>
<p>Keyloggers save keystrokes — website login URLs, passwords, email messages — and send it to attackers, circumventing encryption protections since they capture data at the input stage. Other data logging includes clipboard, screen, IM, and search queries.</p>
</details>

---

### 8. What happened in the March 2013 South Korea logic bomb incident?
- [ ] A worm spread through USB drives across government networks
- [ ] A trojan delivered through a malicious bank email deleted everything, including operating systems, on ATMs and bank machines at a predefined time
- [ ] A DDoS attack took down major South Korean banks
- [ ] A rootkit infected the Windows kernel of every ATM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A trojan delivered through a malicious bank email deleted everything, including operating systems, on ATMs and bank machines at a predefined time</p>
<p>A logic bomb waits for a predefined event (a time bomb or user event). This trojan installed malware via a malicious bank email, then deleted everything the next day at 2pm, killing ATMs and bank machines.</p>
</details>

---

### 9. Why are rootkits so difficult to detect and remove?
- [ ] They only run for a few seconds at a time
- [ ] They modify core system files (part of the kernel) and can be invisible to the OS, task manager, and traditional anti-virus
- [ ] They require physical access to install
- [ ] They only affect mobile devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They modify core system files (part of the kernel) and can be invisible to the OS, task manager, and traditional anti-virus</p>
<p>Removing a rootkit usually requires a remover built specifically for that rootkit after it's discovered, and using secure boot with UEFI helps prevent rootkits from loading in the first place.</p>
</details>

---

### 10. Why is RFID cloning of access badges considered such an easy physical attack?
- [ ] It requires access to the badge's private encryption key
- [ ] Cheap duplicators (under $50) can clone a badge in seconds just by brushing up near someone
- [ ] It requires the badge to be physically disassembled
- [ ] It only works on badges without a chip

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Cheap duplicators (under $50) can clone a badge in seconds just by brushing up near someone</p>
<p>RFID access badges and key fobs are everywhere, and duplicators are cheap and available on Amazon — this is part of why MFA is so important as a second layer of defense.</p>
</details>

---

### 11. Which of the following is an example of an environmental physical attack?
- [ ] Triggering the fire suppression system to cause water damage or force an evacuation
- [ ] Cloning an RFID badge
- [ ] Smashing through a locked door
- [ ] Sending a phishing email

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Triggering the fire suppression system to cause water damage or force an evacuation</p>
<p>Environmental attacks target the operating environment — power monitoring, HVAC/humidity controls (critical for data centers), and fire suppression systems that can flood a space or force an evacuation.</p>
</details>

---

### 12. What is a "friendly" or unintentional denial of service, according to the notes?
- [ ] A DDoS launched by a botnet
- [ ] A network Layer 2 loop from switches without spanning tree, or bandwidth exhaustion from downloading huge files over a slow link
- [ ] An RF jamming attack
- [ ] A deliberate SSL stripping attack

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A network Layer 2 loop from switches without spanning tree, or bandwidth exhaustion from downloading huge files over a slow link</p>
<p>A friendly DoS is unintentional — examples include a Layer 2 switching loop without spanning tree, or bandwidth DoS from downloading multi-gigabyte files over a DSL line.</p>
</details>

---

### 13. Why are NTP, DNS, and ICMP commonly used for DDoS reflection and amplification attacks?
- [ ] They require strong authentication, making them easy to spoof
- [ ] They have little to no authentication checks, and a small request can trigger a much larger response sent to the victim
- [ ] They only operate over UDP port 443
- [ ] They cannot be spoofed at all

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They have little to no authentication checks, and a small request can trigger a much larger response sent to the victim</p>
<p>Reflection and amplification turn a small attack into a big one by using protocols with little authentication, where very little info goes out but a lot more data comes back, directed at the victim.</p>
</details>

---

### 14. Why does modifying a client's host file work as a form of DNS poisoning?
- [ ] The host file requires a valid CA-signed certificate
- [ ] The host file takes precedence over DNS queries
- [ ] The host file is checked only after DNS fails
- [ ] The host file cannot be modified without admin rights

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The host file takes precedence over DNS queries</p>
<p>DNS poisoning can modify the DNS server (uncommon, requires crafty hacking), modify the client host file (which takes precedence over DNS), or send a fake response to a valid DNS request in real time.</p>
</details>

---

### 15. In the October 2016 Brazilian bank incident, how did attackers effectively "become the bank"?
- [ ] They compromised the bank's internal Active Directory server
- [ ] They changed the DNS registrations of 36 domains by gaining access to the domain registration itself
- [ ] They cloned RFID badges to enter the bank's headquarters
- [ ] They used a birthday attack to forge SSL certificates

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They changed the DNS registrations of 36 domains by gaining access to the domain registration itself</p>
<p>Domain hijacking gets access to the domain registration without ever touching the actual servers — via brute force, social engineering, or gaining access to the managing email account.</p>
</details>

---

### 16. What is "typosquatting" an example of?
- [ ] URL hijacking that takes advantage of poor spelling
- [ ] A DDoS amplification technique
- [ ] A rootkit installation method
- [ ] A wireless deauthentication attack

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> URL hijacking that takes advantage of poor spelling</p>
<p>Types of URL hijacking include typosquatting, outright misspellings, typing errors, different phrases, and using a different top-level domain (e.g. .org instead of .gov).</p>
</details>

---

### 17. Why were original 802.11 wireless management frames a security weakness that enabled deauthentication attacks?
- [ ] They were encrypted with a weak cipher
- [ ] They originally had no protection at all
- [ ] They required physical access to send
- [ ] They were only used for QoS management

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They originally had no protection at all</p>
<p>Original wireless standards had no protection for management frames (used to find APs, manage QoS, associate/disassociate). 802.11ac introduced updates encrypting some of these frames, like disassociate and deauth, though not everything is encrypted.</p>
</details>

---

### 18. How does RF jamming cause a denial of service for wireless users?
- [ ] It physically disconnects the Ethernet cable
- [ ] It transmits interfering signals that decrease the signal-to-noise ratio so devices can't hear the good signal
- [ ] It floods the DNS server with requests
- [ ] It exploits a buffer overflow in the AP firmware

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It transmits interfering signals that decrease the signal-to-noise ratio so devices can't hear the good signal</p>
<p>RF jamming is a form of denial of service that prevents wireless communications for anyone nearby. "Reactive jamming" specifically only activates when someone else tries to communicate.</p>
</details>

---

### 19. What makes ARP poisoning possible as an on-path (man-in-the-middle) attack?
- [ ] ARP requires a certificate to respond
- [ ] ARP has no built-in security, allowing an attacker to redirect local subnet traffic through themselves
- [ ] ARP only operates over encrypted channels
- [ ] ARP cannot be spoofed on modern networks

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> ARP has no built-in security, allowing an attacker to redirect local subnet traffic through themselves</p>
<p>On-path attacks redirect your traffic and pass it on to the destination without you knowing. ARP poisoning (spoofing) is an on-path attack limited to the local IP subnet, since ARP has no security.</p>
</details>

---

### 20. What was formerly known as a "man-in-the-browser" attack?
- [ ] An on-path attack where malware on the victim's own computer does the proxy work, waiting for the victim to log into their bank
- [ ] A DNS poisoning attack against a browser's cache
- [ ] A cross-site scripting attack against a browser extension
- [ ] A brute-force attack against browser saved passwords

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An on-path attack where malware on the victim's own computer does the proxy work, waiting for the victim to log into their bank</p>
<p>This on-path browser attack has a huge advantage for attackers: it looks normal to the victim and makes it easy to proxy encrypted traffic since the malware sits inside the browser itself.</p>
</details>

---

### 21. How does a replay attack differ from an on-path attack?
- [ ] A replay attack requires the attacker to be actively in the traffic path at the time of the original transmission
- [ ] A replay attack uses previously captured network data and can be carried out later from a completely different workstation
- [ ] A replay attack only works against wireless networks
- [ ] There is no meaningful difference between the two

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A replay attack uses previously captured network data and can be carried out later from a completely different workstation</p>
<p>Replay attacks need access to raw network data (via a network tap, ARP poisoning, or malware), but the captured info can be replayed later from a different machine — unlike an on-path attack.</p>
</details>

---

### 22. In a "pass the hash" attack, what does the attacker actually capture and reuse?
- [ ] The victim's plaintext password
- [ ] A copy of the authentication request containing the username and hashed password
- [ ] The server's private key
- [ ] The victim's session cookie only

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A copy of the authentication request containing the username and hashed password</p>
<p>The attacker captures a copy of a normal auth request during transmission, then sends their own auth request using that same username and hashed password. This can be mitigated with encryption, salting, or configuring the server to reject the same hash twice in a row.</p>
</details>

---

### 23. What is session hijacking (sidejacking)?
- [ ] Brute-forcing a login form until it succeeds
- [ ] Gaining access to a server using a stolen session ID, often stored in a browser cookie, without needing to log in
- [ ] Sending a fake DNS response to redirect traffic
- [ ] Jamming a wireless signal to force reauthentication

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Gaining access to a server using a stolen session ID, often stored in a browser cookie, without needing to log in</p>
<p>Cookies store info like tracking, personalization, and session management data. Since session IDs are often stored there, stealing one lets an attacker access a server with no login — this is session hijacking (sidejacking).</p>
</details>

---

### 24. What is the best way to prevent session hijacking on a website?
- [ ] Disable all cookies entirely
- [ ] Encrypt end-to-end with HTTPS (or at least end-to-somewhere with a personal VPN)
- [ ] Use only HTTP for faster page loads
- [ ] Block all third-party scripts

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Encrypt end-to-end with HTTPS (or at least end-to-somewhere with a personal VPN)</p>
<p>Preventing session hijacking requires encrypting the connection end-to-end (the server must allow HTTPS, which is common now), or at least end-to-somewhere using a personal VPN to avoid capture until the VPN concentrator.</p>
</details>

---

### 25. What vulnerability did the WannaCry ransomware executable exploit?
- [ ] A flaw in the Windows SMBv1 protocol, enabling arbitrary code execution
- [ ] A SQL injection flaw in a healthcare database
- [ ] A cross-site scripting flaw on a checkout page
- [ ] A weak RFID badge encoding scheme

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A flaw in the Windows SMBv1 protocol, enabling arbitrary code execution</p>
<p>WannaCry's executable exploited a vulnerability in Windows SMBv1, achieving arbitrary code execution — a classic example of malicious code exploiting a system vulnerability.</p>
</details>

---

### 26. In the British Airways breach example, how did attackers steal 380,000 payment cards?
- [ ] By SQL-injecting the payment database directly
- [ ] By injecting about 22 lines of malicious JavaScript onto the checkout pages
- [ ] By cloning employee RFID badges to access servers
- [ ] By exploiting a rootkit in the point-of-sale terminals

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By injecting about 22 lines of malicious JavaScript onto the checkout pages</p>
<p>This was an XSS attack: a small amount of malicious JS on the checkout pages was enough to steal 380,000 cards.</p>
</details>

---

### 27. What kind of attack breached the Estonian Central Health Database, exposing healthcare information for citizens?
- [ ] Cross-site request forgery
- [ ] SQL injection
- [ ] DNS poisoning
- [ ] Rootkit installation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> SQL injection</p>
<p>SQL injection was used to breach all healthcare information held for Estonian citizens in the Central Health Database.</p>
</details>

---

### 28. What is horizontal privilege escalation?
- [ ] A regular user gaining full administrator/root access
- [ ] User A gaining access to User B's resources, where both users have similar privilege levels
- [ ] An attacker escaping a virtual machine to control the host
- [ ] A service account gaining domain admin rights

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> User A gaining access to User B's resources, where both users have similar privilege levels</p>
<p>Privilege escalation vulnerabilities are high-priority patches. Horizontal privilege escalation specifically means User A can access User B's resources, rather than gaining a higher tier of access.</p>
</details>

---

### 29. What does Data Execution Prevention (DEP) do?
- [ ] Prevents any application from writing to disk
- [ ] Only allows data in designated executable areas of memory to actually run
- [ ] Randomizes memory addresses to prevent buffer overruns
- [ ] Blocks all outbound network connections

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Only allows data in designated executable areas of memory to actually run</p>
<p>DEP is a privilege escalation mitigation that ensures only data in executable memory areas can run, distinct from Address Space Layout Randomization (ASLR), which prevents a buffer overrun at a known memory address.</p>
</details>

---

### 30. Why is Cross-Site Request Forgery (CSRF/XSRF) also called a "one-click attack" or "session riding"?
- [ ] It requires the victim to install a malicious browser extension
- [ ] It exploits the trust a web app has in an already-authenticated browser, making unauthorized requests without the victim's consent
- [ ] It requires the attacker to physically click the victim's mouse
- [ ] It only works over unencrypted HTTP connections

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It exploits the trust a web app has in an already-authenticated browser, making unauthorized requests without the victim's consent</p>
<p>A website trusts the browser, so requests can be made without the victim's knowledge (e.g. posting a Facebook status on their behalf). This is a web app development oversight, fixed by adding anti-forgery techniques like a cryptographic token.</p>
</details>

---

### 31. What does a directory traversal attack allow an attacker to do?
- [ ] Redirect DNS queries to a malicious server
- [ ] Read files from a web server that are outside of the website's intended file directory
- [ ] Forge cross-site requests using stolen session tokens
- [ ] Downgrade an HTTPS connection to HTTP

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Read files from a web server that are outside of the website's intended file directory</p>
<p>Directory traversal takes advantage of a web server software vulnerability or badly written web application code to read files a user shouldn't be able to browse, like the Windows folder.</p>
</details>

---

### 32. What real-world probability does a birthday attack exploit in the context of hashing?
- [ ] That two files will always have different hashes
- [ ] That two different inputs may share the same hash output (a collision), similar to two people sharing a birthday in a small group
- [ ] That passwords longer than 8 characters can't be brute forced
- [ ] That all hash algorithms produce the exact same output length

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> That two different inputs may share the same hash output (a collision), similar to two people sharing a birthday in a small group</p>
<p>Just as a class of 23 students has about a 50% chance two share a birthday, a birthday attack looks for a hash collision through brute force, generating plaintext until a hash matches. Using a larger hash output size helps protect against this.</p>
</details>

---

### 33. What does SSL stripping combine to "strip the S away from HTTPS"?
- [ ] A birthday attack with a replay attack
- [ ] An on-path attack with a downgrade attack
- [ ] A DNS poisoning attack with an ARP poisoning attack
- [ ] A pass-the-hash attack with session hijacking

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An on-path attack with a downgrade attack</p>
<p>SSL stripping combines an on-path attack with a downgrade attack, forcing the victim's connection down to unencrypted HTTP. It's difficult to implement since the attacker must sit in the middle of the conversation.</p>
</details>

---

### 34. In a password spraying attack, why does the attacker only try a small number of common passwords per account?
- [ ] To avoid triggering account lockouts, alarms, or alerts while trying that password across many accounts
- [ ] Because spraying always works on the first attempt
- [ ] Because it's required by the hashing algorithm
- [ ] Because only a few passwords exist in the world

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To avoid triggering account lockouts, alarms, or alerts while trying that password across many accounts</p>
<p>Spraying tries the top few common passwords against many accounts (moving to the next account if it fails), unlike brute force, which tries every possible combination against one account.</p>
</details>

---

### 35. Why is offline brute-forcing of passwords much more common than online brute-forcing?
- [ ] Offline attacks are illegal, so attackers prefer online attacks
- [ ] Online attacks are very slow due to lockouts, while offline attacks let an attacker calculate and compare hashes against a stolen list without any lockout restriction
- [ ] Offline attacks require no computing power at all
- [ ] Online attacks always succeed within seconds

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Online attacks are very slow due to lockouts, while offline attacks let an attacker calculate and compare hashes against a stolen list without any lockout restriction</p>
<p>Brute force tries every possible password combination until a hash matches. Offline brute force (using a stolen list of users and hashes) is much more common than online brute force, which is slowed by lockouts.</p>
</details>

---

### 36. What makes "impossible travel" in authentication logs such a clear Indicator of Compromise (IOC)?
- [ ] A user logs in from the same city twice in one day
- [ ] The same user account logs in from two geographically distant locations within a time gap too short for actual travel
- [ ] A user logs in outside of business hours
- [ ] A user changes their password from a new device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The same user account logs in from two geographically distant locations within a time gap too short for actual travel</p>
<p>For example, a login from company HQ in Omaha, NE, followed three minutes later by a login from Australia by the same user, is physically impossible and should be easy to identify in the logs.</p>
</details>

---

### 37. Why is resource consumption (like a 3AM bandwidth spike) often the first real notification that something is wrong?
- [ ] Because attackers always announce their presence beforehand
- [ ] Because every attacker action has an equal and opposite reaction, and firewall logs will show unusual outgoing transfers
- [ ] Because resource consumption never correlates with an attack
- [ ] Because it only occurs after data has already been publicly leaked

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Because every attacker action has an equal and opposite reaction, and firewall logs will show unusual outgoing transfers</p>
<p>File transfers use bandwidth, so unusual traffic spikes (like at 3AM) showing in firewall logs are often the first real notification of an issue.</p>
</details>

---

### 38. Why would an attacker delete or tamper with log information during an intrusion?
- [ ] Logs slow down the system's performance
- [ ] Log info is evidence, and attackers want to avoid leaving an incriminating trail
- [ ] Logs are required to be deleted under compliance rules
- [ ] Deleting logs automatically fixes the vulnerability they exploited

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Log info is evidence, and attackers want to avoid leaving an incriminating trail</p>
<p>Missing logs are an IOC — since log info can be incriminating evidence everywhere, it's important to set up notifications if any log info goes missing.</p>
</details>

---

### 39. What does it mean when a company's data becomes an IOC through being "published/documented"?
- [ ] The company published a transparency report
- [ ] An attacker posts a portion or all of the stolen data online, sometimes alongside a ransomware attack
- [ ] The company documented the incident in their SOC runbook
- [ ] Security researchers published a CVE about the vulnerability

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An attacker posts a portion or all of the stolen data online, sometimes alongside a ransomware attack</p>
<p>The entire attack may otherwise go unnoticed until the IOC is that company data becomes available online — the attacker may release raw data without context, sometimes in conjunction with a ransomware attack.</p>
</details>
