# Quiz 2.3 — Memory Injections
*Professor Messer SY0-701 · Section 2.3*

---

### 1. Why can memory forensics be used to find malware?
- [ ] Malware is always stored in the registry
- [ ] Malware must run in memory, where it exists as running processes
- [ ] Malware can only spread through memory dumps
- [ ] Memory forensics decrypts the malware's payload on disk

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Malware must run in memory, where it exists as running processes</p>
<p>Malware runs in memory, so memory forensics can find malicious code there. Malware can run its own process or inject itself into a legitimate process.</p>
</details>

---

### 2. What is a memory injection attack?
- [ ] Overwriting a buffer so it spills into adjacent memory
- [ ] Adding code into the memory of an existing process to access its data and hide within it
- [ ] Replacing a DLL on disk with an older version
- [ ] Filling system memory until the machine crashes

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Adding code into the memory of an existing process to access its data and hide within it</p>
<p>Memory injection adds code into an existing process's memory, giving access to that process's data while hiding in the process, and can be used to perform a privilege escalation.</p>
</details>

---

### 3. In a DLL injection, what does the attacker do?
- [ ] Deletes the target process's DLL files
- [ ] Injects a path to a malicious DLL so it runs as part of the target process
- [ ] Encrypts the DLL so the process can't load it
- [ ] Downloads a DLL from the vendor's official site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Injects a path to a malicious DLL so it runs as part of the target process</p>
<p>A Dynamic-Link Library (DLL) is a Windows library containing code and data many apps can use. DLL injection is very popular and relatively easy to implement.</p>
</details>

---

### 4. What is a buffer overflow?
- [ ] Two events occurring at nearly the same time that the app doesn't account for
- [ ] Overwriting a buffer of memory so that data spills over into other memory areas
- [ ] Adding your own SQL requests to an existing application
- [ ] Breaking out of a virtual machine to reach the host

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Overwriting a buffer of memory so that data spills over into other memory areas</p>
<p>In a buffer overflow, a buffer is overwritten and spills into other memory areas. Developers need to perform bounds checking, and attackers spend time looking for openings.</p>
</details>

---

### 5. Which type of buffer overflow is especially useful to an attacker?
- [ ] One that always crashes the system
- [ ] One that is always repeatable
- [ ] One that only works once
- [ ] One that triggers bounds checking

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> One that is always repeatable</p>
<p>Buffer overflows aren't simple exploits — they can cause crashes and take time to make work perfectly, so an overflow that is always repeatable is very useful to an attacker.</p>
</details>

---

### 6. What does TOCTOU stand for, and what does it describe?
- [ ] Time-of-check to time-of-use; something can change between checking the system and using the result of that check
- [ ] Type-of-content to type-of-usage; a mismatch between file types
- [ ] Token-of-control to token-of-usage; stolen session tokens
- [ ] Time-of-connection to time-of-upload; delays in data transfer

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Time-of-check to time-of-use; something can change between checking the system and using the result of that check</p>
<p>TOCTOU is a race condition attack. You check the system, then later use the result of that check — but something might happen between the check and the use.</p>
</details>

---

### 7. In the race condition example from the notes, why did Account A end up with a balance that should have been $0?
- [ ] The bank's database was encrypted incorrectly
- [ ] The balance was never checked a second time after the first check
- [ ] The account was hit by a DLL injection
- [ ] The password was stored without a salt

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The balance was never checked a second time after the first check</p>
<p>The app didn't account for two events running simultaneously, so the balance check went stale between the check and its use.</p>
</details>

---

### 8. In the 2020 SolarWinds Orion supply chain attack, why was the malicious update still trusted by customers?
- [ ] The update was unsigned but downloaded from the vendor's site
- [ ] Attackers added malicious code to the software updates, which the company then digitally signed
- [ ] The update used an outdated version of TLS
- [ ] Customers manually sideloaded the update

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Attackers added malicious code to the software updates, which the company then digitally signed</p>
<p>Automatic updates are relatively trustworthy since they include security checks and digital signatures, but in this attack the malicious code was added before the company signed the update.</p>
</details>

---

### 9. Why are operating systems such attractive targets for attackers?
- [ ] They are rarely updated
- [ ] Everyone has one, and their millions of lines of code create more opportunities for vulnerabilities
- [ ] They don't support firewalls
- [ ] They are always end-of-life

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Everyone has one, and their millions of lines of code create more opportunities for vulnerabilities</p>
<p>An operating system is a foundational computing platform, very attractive to attackers since everyone has one, and remarkably complex.</p>
</details>

---

### 10. When does "Patch Tuesday" occur for Windows?
- [ ] Every Tuesday
- [ ] The 1st Tuesday of each month
- [ ] The 2nd Tuesday of each month
- [ ] The last Tuesday of each quarter

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The 2nd Tuesday of each month</p>
<p>Patch Tuesday for Windows falls on the 2nd Tuesday each month; in April 2023 nearly 100 vulnerabilities were patched, and nearly 50 in May 2023.</p>
</details>

---

### 11. Which of the following is a best practice for handling OS vulnerabilities?
- [ ] Never reboot after patching
- [ ] Always update, but test before deployment if needed and have a fallback plan
- [ ] Delay all updates for one year
- [ ] Only update after an attack occurs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Always update, but test before deployment if needed and have a fallback plan</p>
<p>It's a race between you and the attackers, so always update. Updates may need testing (they may break something else), may require a reboot, and you should have a fallback plan.</p>
</details>

---

### 12. What does entering `3SL99A' OR '1' = '1` into a vulnerable search field accomplish in the SQL injection example?
- [ ] It logs the attacker out of the database
- [ ] The extra condition is always true, so the code runs it as SQL and returns a full list of database info
- [ ] It encrypts the database with a new key
- [ ] It causes a DLL to be loaded

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The extra condition is always true, so the code runs it as SQL and returns a full list of database info</p>
<p>SQL injection puts your own SQL requests into an existing application, which shouldn't be allowed. It's enabled by bad programming and is often not difficult to exploit, sometimes just through a browser.</p>
</details>

---

### 13. What is cross-site scripting (XSS) commonly built on?
- [ ] JavaScript
- [ ] SQL
- [ ] Assembly
- [ ] IPsec

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> JavaScript</p>
<p>XSS was originally called "cross-site" because of browser security flaws that let info from one site be shared with another, and it commonly uses JavaScript.</p>
</details>

---

### 14. What describes a non-persistent (reflected) XSS attack?
- [ ] The malicious payload is posted to a social network and everyone who loads the page gets it
- [ ] The attacker emails a link with a script embedded in the URL that executes in the victim's browser and reflects data back in a single response
- [ ] The attacker overwrites memory beyond a buffer
- [ ] The attacker changes the DNS record for a site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The attacker emails a link with a script embedded in the URL that executes in the victim's browser and reflects data back in a single response</p>
<p>The website allows scripts to run in user input. The attacker can then use credentials, session IDs, or cookies to steal the victim's info without their knowledge.</p>
</details>

---

### 15. What makes a persistent (stored) XSS attack "persistent"?
- [ ] It targets one specific victim
- [ ] The payload stays on the site, so everyone gets it once they load the page, with no specific target
- [ ] It survives a reboot of the victim's machine
- [ ] It requires the victim to click a link each time

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The payload stays on the site, so everyone gets it once they load the page, with no specific target</p>
<p>For example, an attacker posts a message to a social network containing the malicious payload. Reposts can amplify the effect.</p>
</details>

---

### 16. Why can only the vendor fix firmware vulnerabilities in their hardware?
- [ ] Firmware can't be updated
- [ ] They know the software, the OS, and the device, since firmware is the operating system inside the hardware
- [ ] Firmware is always open source
- [ ] Firmware is stored in the cloud

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They know the software, the OS, and the device, since firmware is the operating system inside the hardware</p>
<p>Firmware is the operating system inside the hardware, and vendors are the only ones who can fix their hardware.</p>
</details>

---

### 17. Which date matters more for security: end-of-life (EOL) or end of service life (EOSL)?
- [ ] EOL, because the product is no longer sold
- [ ] EOSL, because support ends and there are no more security patches or updates
- [ ] Neither, since patches continue forever
- [ ] They mean exactly the same thing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> EOSL, because support ends and there are no more security patches or updates</p>
<p>EOL means the manufacturer stops selling a product (support may continue for a while). EOSL means support is no longer available. EOSL is the more important date, while EOL is a good reminder to upgrade.</p>
</details>

---

### 18. What additional protections might legacy platforms running EOL software require?
- [ ] Removing all firewall rules
- [ ] Additional firewall rules and IPS signatures for older operating systems
- [ ] Disabling all logging
- [ ] Sideloading new apps

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Additional firewall rules and IPS signatures for older operating systems</p>
<p>Legacy devices run older operating systems, apps, and middleware. Their risk should be compared to their return, and they may require additional security protections.</p>
</details>

---

### 19. What is a virtual machine escape?
- [ ] Moving a VM from one host to another
- [ ] Breaking out of the VM to interact with the host OS or hardware, and potentially control other guest VMs
- [ ] Deleting a VM snapshot
- [ ] Allocating more RAM to a VM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Breaking out of the VM to interact with the host OS or hardware, and potentially control other guest VMs</p>
<p>A VM is supposed to be self-contained, but once an attacker escapes they have great control — of the host and of other guest VMs.</p>
</details>

---

### 20. What does the hypervisor manage that creates a resource reuse risk between VMs?
- [ ] Certificates and revocation lists
- [ ] The relationship between physical and virtual resources (RAM, storage, CPU), where resources can be reused between VMs and data may inadvertently be shared
- [ ] Wireless authentication
- [ ] Email routing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The relationship between physical and virtual resources (RAM, storage, CPU), where resources can be reused between VMs and data may inadvertently be shared</p>
<p>For example, a host with 4GB of RAM can run three 2GB VMs because RAM is allocated and shared between them. Data can inadvertently be shared, which is a security risk.</p>
</details>

---

### 21. Which cloud-specific attack takes advantage of faulty configurations that let an attacker manually move around the structure of a web server?
- [ ] Directory traversal
- [ ] Authentication bypass
- [ ] Remote code execution
- [ ] Denial of service

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Directory traversal</p>
<p>Attacks on the service include denial of service, authentication bypass (weak/faulty auth), directory traversal (faulty configs put data at risk), and remote code execution (unpatched systems).</p>
</details>

---

### 22. In the 2013 Target breach, what type of supply chain weakness was exploited?
- [ ] A counterfeit Cisco switch
- [ ] A trusted service provider (an AC contractor) with access to internal services
- [ ] A malicious software update
- [ ] An unpatched zero-day

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A trusted service provider (an AC contractor) with access to internal services</p>
<p>Service providers often have access to internal services, which is an opportunity for attackers. Consider ongoing security audits of all providers, included in the contract.</p>
</details>

---

### 23. How can an organization gain tighter control over hardware providers?
- [ ] Buy from as many suppliers as possible
- [ ] Use a small supplier base with strict controls over policies and procedures
- [ ] Only buy used equipment
- [ ] Skip verification of software signatures

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Use a small supplier base with strict controls over policies and procedures</p>
<p>You need to be able to trust your new server, router, switch, firewall, or software. Cisco knockoffs were sold often, but then they break.</p>
</details>

---

### 24. What happened in the 2017 Verizon example of open permissions?
- [ ] An attacker guessed a root password
- [ ] 14 million records were exposed through an Amazon S3 data repository
- [ ] A zero-day was used to break out of a VM
- [ ] A SQL injection dumped a payroll database

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> 14 million records were exposed through an Amazon S3 data repository</p>
<p>Open permissions leave info in an open area of the internet, and are increasingly common with cloud storage.</p>
</details>

---

### 25. What is the recommended way to protect the Linux root account?
- [ ] Enable direct login to root with a simple password
- [ ] Disable direct login to root and use su or sudo instead
- [ ] Share the password with all admins
- [ ] Rename the account to "admin"

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Disable direct login to root and use su or sudo instead</p>
<p>Unsecured admin accounts (Linux root, Windows admin, superuser) can be misconfigurations, such as intentionally configuring an easy-to-hack password. Protect accounts with root/admin access.</p>
</details>

---

### 26. Which of these are insecure, unencrypted protocols, and what are their encrypted alternatives?
- [ ] SSH, SFTP, IMAPS; alternatives are Telnet, FTP, IMAP
- [ ] Telnet, FTP, SMTP, IMAP; alternatives include SSH, SFTP, IMAPS
- [ ] HTTPS, SSH, TLS; alternatives are HTTP, FTP, SMTP
- [ ] SNMP, DNS, NTP; alternatives are Telnet, FTP, IMAP

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Telnet, FTP, SMTP, IMAP; alternatives include SSH, SFTP, IMAPS</p>
<p>Some protocols aren't encrypted. Verify with a packet capture and use the encrypted versions.</p>
</details>

---

### 27. How did the Mirai botnet spread to IoT devices?
- [ ] By exploiting zero-day vulnerabilities in firmware
- [ ] By taking advantage of default configurations and logins
- [ ] By jailbreaking the devices
- [ ] By sideloading apps

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By taking advantage of default configurations and logins</p>
<p>Every app and network device has a default login. The Mirai botnet took advantage of default configs for IoT devices and was released as open-source software.</p>
</details>

---

### 28. Why does jailbreaking or rooting a mobile device make a Mobile Device Manager (MDM) relatively useless?
- [ ] It removes the device's battery
- [ ] It gives uncontrolled access that can circumvent security features
- [ ] It forces the device to use a VPN
- [ ] It only works on tablets

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It gives uncontrolled access that can circumvent security features</p>
<p>Rooting (Android) or jailbreaking (iOS) installs custom firmware to replace the existing OS, circumventing security features and making the MDM useless.</p>
</details>

---

### 29. What is sideloading?
- [ ] Installing apps manually without using an app store
- [ ] Loading a website in a second browser tab
- [ ] Backing up a phone to a PC
- [ ] Updating firmware over Wi-Fi

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Installing apps manually without using an app store</p>
<p>Malicious apps are a significant concern — one trojan horse can cause a data breach. Manage installation sources; sideloading also makes the MDM relatively useless.</p>
</details>

---

### 30. What defines a zero-day attack?
- [ ] An attack that happens on the first day of the month
- [ ] An attack on an unknown vulnerability with no patch or method of mitigation, since the vendor doesn't know it exists
- [ ] An attack that takes zero seconds to complete
- [ ] An attack using a previously patched vulnerability

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An attack on an unknown vulnerability with no patch or method of mitigation, since the vendor doesn't know it exists</p>
<p>Someone is always working hard to find the next big vulnerability, to report it or exploit it for personal gain. It's a race to exploit the vulnerability or create a patch.</p>
</details>
