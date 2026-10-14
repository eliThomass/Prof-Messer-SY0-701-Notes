# Quiz 4.1 — Secure Baselines
*Professor Messer SY0-701 · Section 4.1*

---

### 1. What is a security baseline?
- [ ] A one-time security scan
- [ ] A well-defined security standard for an application environment (firewall settings, patch levels, OS versions) that all app instances must follow
- [ ] The default configuration a system ships with
- [ ] A list of known attackers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A well-defined security standard for an application environment (firewall settings, patch levels, OS versions) that all app instances must follow</p>
<p>Baselines may require constant updates and should be checked constantly. A failure requires immediate correction.</p>
</details>

---

### 2. Where do many organizations get a starting point for their security baselines?
- [ ] They must always write them from scratch
- [ ] From foundational baselines created by application developers, OS manufacturers, and appliance manufacturers, which can be changed to fit the organization
- [ ] From their competitors
- [ ] From end users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> From foundational baselines created by application developers, OS manufacturers, and appliance manufacturers, which can be changed to fit the organization</p>
<p>Many operating systems have extensive options — Windows 10 has over 3,000 group policy settings, though only a subset are for security.</p>
</details>

---

### 3. What is key when deploying baselines?
- [ ] Doing everything manually
- [ ] Automation, usually managed through an admin console, sometimes with multiple deployment mechanisms
- [ ] Only deploying to one system
- [ ] Letting users choose their own settings

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Automation, usually managed through an admin console, sometimes with multiple deployment mechanisms</p>
<p>Automating deployment keeps baselines consistent across many systems.</p>
</details>

---

### 4. Why should you test and measure when maintaining baselines?
- [ ] Baselines never change
- [ ] Some settings contradict each other, so testing helps avoid conflicts
- [ ] Testing is only needed for new hardware
- [ ] To remove all best practices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Some settings contradict each other, so testing helps avoid conflicts</p>
<p>Many baseline settings are best practices that rarely change, but some need ongoing updates.</p>
</details>

---

### 5. Why is hardening necessary for every system?
- [ ] No system is secure with its default configuration
- [ ] Default configurations are always secure
- [ ] Hardening only applies to servers
- [ ] Hardening removes the need for patches

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> No system is secure with its default configuration</p>
<p>Hardening guides are specific to the software or platform and come from the manufacturer or the internet.</p>
</details>

---

### 6. How can segmentation help harden mobile devices?
- [ ] By separating company data and user data
- [ ] By disabling all apps
- [ ] By removing the cellular radio
- [ ] By sharing data across all users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By separating company data and user data</p>
<p>Always-connected mobile devices must be hardened with manufacturer patches (which include security updates), segmentation, and control through an MDM.</p>
</details>

---

### 7. Which of these is a workstation hardening practice?
- [ ] Never patching the OS
- [ ] Automating monthly patches, connecting to a policy management system, and removing unnecessary software
- [ ] Installing as much software as possible
- [ ] Disabling all monitoring

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Automating monthly patches, connecting to a policy management system, and removing unnecessary software</p>
<p>Workstations need constant monitoring and updates to the OS, apps, and firmware.</p>
</details>

---

### 8. Why is hardening network infrastructure devices (switches, routers) different from hardening a workstation?
- [ ] They usually use an embedded OS with limited OS access, so you configure authentication, avoid default creds, and check the manufacturer for patches
- [ ] They can't be hardened at all
- [ ] They run full desktop operating systems
- [ ] They don't need authentication

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They usually use an embedded OS with limited OS access, so you configure authentication, avoid default creds, and check the manufacturer for patches</p>
<p>With limited OS access, hardening these devices relies on configuration and manufacturer patches.</p>
</details>

---

### 9. Which of the following is a cloud infrastructure hardening practice?
- [ ] Leave the cloud management workstation unsecured
- [ ] Secure the cloud management workstation, apply least privilege, configure EDR, and keep backups (like cloud to cloud)
- [ ] Give all services full admin rights
- [ ] Skip backups since the cloud never fails

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Secure the cloud management workstation, apply least privilege, configure EDR, and keep backups (like cloud to cloud)</p>
<p>Least privilege should apply to all services, network settings, and app rights.</p>
</details>

---

### 10. Which of these is part of server hardening?
- [ ] Removing password requirements
- [ ] OS updates/service packs, minimum password length and complexity, account limitations, and limited network access
- [ ] Opening all network ports
- [ ] Using default admin accounts

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> OS updates/service packs, minimum password length and complexity, account limitations, and limited network access</p>
<p>Servers are hardened through updates, user account controls, and limits on network access.</p>
</details>

---

### 11. How should SCADA/ICS systems be hardened?
- [ ] Connect them directly to the internet
- [ ] Extensive segmentation with no outside access at all
- [ ] Allow remote access for all users
- [ ] Run them on the same network as workstations

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Extensive segmentation with no outside access at all</p>
<p>SCADA systems are large-scale, multi-site Industrial Control Systems managing equipment like power generation, refining, and manufacturing.</p>
</details>

---

### 12. How should embedded systems that aren't easily modified be protected?
- [ ] Leave them unprotected
- [ ] Apply security patches where possible, and segment and firewall them to prevent unauthorized access
- [ ] Replace their OS with Windows
- [ ] Connect them to a public Wi-Fi network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Apply security patches where possible, and segment and firewall them to prevent unauthorized access</p>
<p>Embedded systems can be difficult to upgrade. Watches and TVs are relatively easy, but other devices may not be easily modified.</p>
</details>

---

### 13. Which of the following is a way to harden a Real-Time Operating System (RTOS)?
- [ ] Run as many services as possible
- [ ] Isolate it from the rest of the network, run minimum services, and use secure communication with a host-based firewall
- [ ] Give it direct internet access
- [ ] Disable all firewalls

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Isolate it from the rest of the network, run minimum services, and use secure communication with a host-based firewall</p>
<p>An RTOS has a deterministic processing schedule with no time to wait for other processes, so it's run with minimal services to reduce exploit potential.</p>
</details>

---

### 14. What is a recommended way to segment IoT devices?
- [ ] Put them on their own VLAN
- [ ] Put them on the same network as servers
- [ ] Give them public IP addresses
- [ ] Connect them through Bluetooth only

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Put them on their own VLAN</p>
<p>IoT devices (heating/cooling, lighting, home automation, wearables) often have weak defaults, so change passwords, deploy updates quickly, and segment them.</p>
</details>

---

### 15. What is the purpose of a wireless site survey?
- [ ] To install new access points without planning
- [ ] To determine the existing wireless landscape by sampling the spectrum (with a heat map), identifying all APs, and planning around interference
- [ ] To check employee badges
- [ ] To test phishing awareness

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To determine the existing wireless landscape by sampling the spectrum (with a heat map), identifying all APs, and planning around interference</p>
<p>Plan for ongoing site surveys at regular intervals.</p>
</details>

---

### 16. Which tool shows you all the signals on a particular frequency?
- [ ] Spectrum analyzer
- [ ] Static code analyzer
- [ ] Fuzzer
- [ ] RADIUS server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Spectrum analyzer</p>
<p>Wireless survey tools give a signal coverage overview and show potential interference. You can use tools built into your OS or third-party tools like NetSpot.</p>
</details>

---

### 17. What can a Mobile Device Manager (MDM) do?
- [ ] Only track device location
- [ ] Centrally manage company-owned and user-owned devices, set policies on apps, data, and camera, create business partitions, and force screen locks and PINs
- [ ] Only manage desktop computers
- [ ] Replace the device's operating system

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Centrally manage company-owned and user-owned devices, set policies on apps, data, and camera, create business partitions, and force screen locks and PINs</p>
<p>MDMs work for both corporate-owned devices and BYOD.</p>
</details>

---

### 18. Why is BYOD (Bring Your Own Device) difficult to secure?
- [ ] The company owns the device
- [ ] The device is both a home and work device, so you must protect two sides of the data, including if the phone is traded in
- [ ] BYOD devices can't connect to the network
- [ ] BYOD devices don't need to meet company requirements

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The device is both a home and work device, so you must protect two sides of the data, including if the phone is traded in</p>
<p>With BYOD, the employee owns the device, but it must meet the company's requirements.</p>
</details>

---

### 19. What does COPE stand for, and who owns the device?
- [ ] Corporate Owned, Personally Enabled — the company buys and controls the device, but employees can also use it personally
- [ ] Choose Our Phone Easily — the employee buys it
- [ ] Corporate Operated, Privately Encrypted — a third party owns it
- [ ] Company Optional Personal Equipment — no one owns it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Corporate Owned, Personally Enabled — the company buys and controls the device, but employees can also use it personally</p>
<p>The org keeps full control, similar to company-owned laptops, and info is protected by corporate policies and can be deleted at any time.</p>
</details>

---

### 20. What is CYOD?
- [ ] Choose Your Own Device — the employee chooses which corporate-owned device to use
- [ ] Control Your Own Data — users manage their own security
- [ ] Copy Your Own Device — a backup method
- [ ] Connect Your Own Device — any device can join the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Choose Your Own Device — the employee chooses which corporate-owned device to use</p>
<p>CYOD is a variation of corporate ownership where the employee picks the device.</p>
</details>

---

### 21. On Wi-Fi, if encrypting all data isn't possible, what should you use?
- [ ] An open network
- [ ] A VPN
- [ ] Bluetooth
- [ ] A spectrum analyzer

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A VPN</p>
<p>Wi-Fi threats include on-path (MITM) attacks that modify or monitor data, and denial of service through frequency interference.</p>
</details>

---

### 22. What is the main security recommendation for Bluetooth?
- [ ] Always leave it discoverable
- [ ] Don't connect to unknown Bluetooth devices
- [ ] Use it instead of Wi-Fi for everything
- [ ] Disable all encryption

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Don't connect to unknown Bluetooth devices</p>
<p>Bluetooth creates a PAN (Personal Area Network) to connect mobile devices.</p>
</details>

---

### 23. Which of the following is a goal of securing a wireless network?
- [ ] Allowing anyone to connect without authentication
- [ ] Authenticating users before access, keeping communication confidential, and verifying integrity with a message integrity check (MIC)
- [ ] Broadcasting the password publicly
- [ ] Disabling all encryption for speed

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Authenticating users before access, keeping communication confidential, and verifying integrity with a message integrity check (MIC)</p>
<p>Users authenticate with a username, password, and MFA before getting access.</p>
</details>

---

### 24. What is the WPA2 PSK problem?
- [ ] WPA2 doesn't use a pre-shared key
- [ ] Attackers can capture the PSK hash (from the 4-way handshake or other methods) and brute force it, and once they have the PSK they have everyone's wireless key
- [ ] WPA2 encrypts too slowly
- [ ] WPA2 only works on wired networks

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Attackers can capture the PSK hash (from the 4-way handshake or other methods) and brute force it, and once they have the PSK they have everyone's wireless key</p>
<p>This brute-force attack is becoming even easier as devices get faster.</p>
</details>

---

### 25. What does GCMP provide in WPA3?
- [ ] Galois/Counter Mode Protocol — data confidentiality with AES and a MIC using Galois Message Authentication Code (GMAC)
- [ ] A 4-way handshake for authentication
- [ ] Open authentication with no encryption
- [ ] A centralized authentication server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Galois/Counter Mode Protocol — data confidentiality with AES and a MIC using Galois Message Authentication Code (GMAC)</p>
<p>GCMP is a block cipher mode that provides better encryption for WPA3.</p>
</details>

---

### 26. How does SAE (Simultaneous Authentication of Equals) in WPA3 fix the WPA2 PSK problem?
- [ ] It sends the session key across the network in plaintext
- [ ] It uses mutual authentication and a Diffie-Hellman derivation to create a shared session key without sending it, with no 4-way handshake, and every user gets a different session key even with the same PSK
- [ ] It removes all authentication
- [ ] It uses the same session key for everyone

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It uses mutual authentication and a Diffie-Hellman derivation to create a shared session key without sending it, with no 4-way handshake, and every user gets a different session key even with the same PSK</p>
<p>SAE is an IEEE standard, and with no more 4-way handshake there are no more handshake attacks.</p>
</details>

---

### 27. What is the difference between WPA3-Personal and WPA3-Enterprise?
- [ ] WPA3-Personal uses a PSK (everyone shares the same 256-bit key); WPA3-Enterprise authenticates users individually with an authentication server (802.1X)
- [ ] WPA3-Enterprise requires no authentication
- [ ] WPA3-Personal uses an authentication server
- [ ] They're identical

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> WPA3-Personal uses a PSK (everyone shares the same 256-bit key); WPA3-Enterprise authenticates users individually with an authentication server (802.1X)</p>
<p>An open system requires no authentication at all.</p>
</details>

---

### 28. In the AAA framework, what does accounting track?
- [ ] Who you claim to be
- [ ] Proof of your identity
- [ ] What access you have
- [ ] The data you used and your login/logout times

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The data you used and your login/logout times</p>
<p>Identification is who you claim to be, authentication proves it, authorization determines your access, and accounting logs your usage.</p>
</details>

---

### 29. What is RADIUS?
- [ ] A wireless encryption cipher
- [ ] Remote Authentication Dial-In User Service, a common AAA protocol that centralizes authentication for routers, switches, firewalls, servers, VPN access, and 802.1X
- [ ] A type of spectrum analyzer
- [ ] A mobile device manager

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Remote Authentication Dial-In User Service, a common AAA protocol that centralizes authentication for routers, switches, firewalls, servers, VPN access, and 802.1X</p>
<p>RADIUS is available on almost any server OS and is often used as the access database for 802.1X.</p>
</details>

---

### 30. What is input validation, and what is normalization?
- [ ] Checking actual input against what's expected; normalization is checking and correcting input (e.g. a zip code should only have 5 characters)
- [ ] Encrypting all user input
- [ ] Deleting all user input
- [ ] Signing input with a private key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Checking actual input against what's expected; normalization is checking and correcting input (e.g. a zip code should only have 5 characters)</p>
<p>Document all input methods. Attackers use fuzzers, which put random types of data into input fields to try to exploit them.</p>
</details>

---

### 31. What does the "secure" attribute on a cookie do?
- [ ] Encrypts the cookie with AES
- [ ] Ensures the cookie is only sent over HTTPS
- [ ] Makes the cookie executable
- [ ] Allows sensitive info to be stored safely in it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Ensures the cookie is only sent over HTTPS</p>
<p>Cookies are used for tracking, session management, and personalization. They aren't usually a security risk or executable, but sensitive info shouldn't be saved in one.</p>
</details>

---

### 32. What is a limitation of Static Application Security Testing (SAST)?
- [ ] It can't find any vulnerabilities
- [ ] Not everything can be identified through analysis, and each finding still has to be verified
- [ ] It only works on hardware
- [ ] It requires the app to be running in production

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Not everything can be identified through analysis, and each finding still has to be verified</p>
<p>Static code analyzers can easily find many security vulnerabilities, but they aren't perfect.</p>
</details>

---

### 33. How does code signing let users confirm an app hasn't been modified and came from a specific developer?
- [ ] The developer signs the code with their private key, and a trusted CA has signed the developer's public key
- [ ] The developer emails the code to each user
- [ ] The app is hashed with MD5 only
- [ ] The user signs the code with their own private key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The developer signs the code with their private key, and a trusted CA has signed the developer's public key</p>
<p>Code signing uses asymmetric encryption to verify an app's integrity and origin.</p>
</details>

---

### 34. What is sandboxing, and where is it used?
- [ ] Letting apps access all system resources
- [ ] Preventing apps from accessing unrelated resources — used in development and in VMs, mobile devices, browser iframes, and Windows UAC
- [ ] Deleting apps after each use
- [ ] Running apps only on servers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Preventing apps from accessing unrelated resources — used in development and in VMs, mobile devices, browser iframes, and Windows UAC</p>
<p>Sandboxing is common during development, but it can also be useful in production, like staging.</p>
</details>

---

### 35. What can application security monitoring help you do?
- [ ] Only track user logins
- [ ] View blocked attacks (like SQL injection), audit logs to find unknown vulnerabilities or hidden attacks, and detect anomalies like unusual file transfers
- [ ] Replace input validation
- [ ] Sign application code

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> View blocked attacks (like SQL injection), audit logs to find unknown vulnerabilities or hidden attacks, and detect anomalies like unusual file transfers</p>
<p>Application security monitoring provides real-time info from app usage.</p>
</details>
