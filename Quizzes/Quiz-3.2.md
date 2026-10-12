# Quiz 3.2 — Secure Infrastructures
*Professor Messer SY0-701 · Section 3.2*

---

### 1. What is the primary role of a firewall when it comes to device placement?
- [ ] To balance load across servers
- [ ] To separate trusted networks from untrusted networks
- [ ] To cache web content
- [ ] To authenticate wireless users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To separate trusted networks from untrusted networks</p>
<p>Every network is different, but firewalls separate trusted from untrusted. Other services may need their own security technologies, like honeypots, jump servers, load balancers, and sensors.</p>
</details>

---

### 2. Why are zone-based security technologies preferred over IP address ranges?
- [ ] They're more flexible and simplify security policies
- [ ] They require no configuration at all
- [ ] They only work on wireless networks
- [ ] They remove the need for firewalls

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They're more flexible and simplify security policies</p>
<p>Each section of the network is assigned a zone, such as trusted/untrusted, internal/external, or inside, internet, servers, databases, and screened. Policies can then be written between zones (e.g. untrusted to screened).</p>
</details>

---

### 3. Which of the following is a way to minimize the attack surface?
- [ ] Open more ports for flexibility
- [ ] Audit the code, block ports on the firewall, and monitor network traffic in real time
- [ ] Disable logging
- [ ] Give all users admin access

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Audit the code, block ports on the firewall, and monitor network traffic in real time</p>
<p>The attack surface is how many ways there are into the network. Everything can be a vulnerability, including app code, open ports, authentication errors, and human error.</p>
</details>

---

### 4. Why does application-level encryption help even if an attacker captures packets?
- [ ] It blocks the capture entirely
- [ ] The attacker can't know what's inside the encrypted packets
- [ ] It makes the packets smaller
- [ ] It automatically alerts the IPS

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The attacker can't know what's inside the encrypted packets</p>
<p>Everything contributes to security, including the connection: secure network cabling (protect the physical drops), application-level encryption, and network-level encryption like IPsec tunnels and VPNs.</p>
</details>

---

### 5. What is the difference between an IDS and an IPS?
- [ ] An IDS stops intrusions; an IPS only alerts
- [ ] An IDS raises an alarm or alert; an IPS stops the intrusion before it gets into the network
- [ ] They are exactly the same
- [ ] An IPS only works on wireless networks

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An IDS raises an alarm or alert; an IPS stops the intrusion before it gets into the network</p>
<p>Both watch network traffic for intrusions, such as exploits against operating systems and apps.</p>
</details>

---

### 6. If a security device is configured to "fail-open," what happens when it fails?
- [ ] Data stops flowing
- [ ] Data continues to flow
- [ ] The device reboots into a secure mode
- [ ] All users are logged out

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data continues to flow</p>
<p>Fail-open keeps data flowing when the system fails. Fail-closed stops all data from flowing when the system fails.</p>
</details>

---

### 7. What makes active monitoring different from passive monitoring?
- [ ] Active monitoring is connected inline and can block data in real time; passive monitoring examines a copy of the traffic and can't block in real time
- [ ] Passive monitoring is inline; active monitoring uses a tap
- [ ] Active monitoring only examines logs after the fact
- [ ] There's no difference

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Active monitoring is connected inline and can block data in real time; passive monitoring examines a copy of the traffic and can't block in real time</p>
<p>Active monitoring is often the default IPS config, though there's concern over downtime or an overly aggressive IPS. Passive monitoring uses a tap or port monitor and is often called an IDS design since it can't block traffic.</p>
</details>

---

### 8. What is a jump server used for?
- [ ] Caching web pages for users
- [ ] Providing an access mechanism into secure network zones — you SSH to the jump server, then jump to other internal servers
- [ ] Distributing load across a web farm
- [ ] Filtering spam email

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Providing an access mechanism into secure network zones — you SSH to the jump server, then jump to other internal servers</p>
<p>A jump server must be a highly secure device, since it's a significant security concern if compromised.</p>
</details>

---

### 9. Which of the following is NOT a typical use of a proxy server?
- [ ] Caching info
- [ ] Access control and URL filtering
- [ ] Content scanning
- [ ] Providing an always-on site-to-site tunnel

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Providing an always-on site-to-site tunnel</p>
<p>A proxy sits between users and the external network, receiving user requests and sending them on their behalf. It's useful for caching, access control, URL filtering, and content scanning.</p>
</details>

---

### 10. What is the difference between an explicit proxy and a transparent proxy?
- [ ] With an explicit proxy, apps need to know how to use the proxy; a transparent proxy is invisible to users
- [ ] A transparent proxy requires every app to be configured
- [ ] An explicit proxy is always invisible
- [ ] They're the same

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> With an explicit proxy, apps need to know how to use the proxy; a transparent proxy is invisible to users</p>
<p>Applications have to be configured for an explicit proxy, while a transparent proxy requires no client configuration.</p>
</details>

---

### 11. What is one of the simplest forms of proxy?
- [ ] NAT
- [ ] A WAF
- [ ] A UTM
- [ ] SASE

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> NAT</p>
<p>NAT is one of the simplest proxies, but most proxies in use are application proxies. An application proxy may know only one app (like HTTP) or several (HTTP, HTTPS, FTP, etc.).</p>
</details>

---

### 12. What does a forward proxy (internal proxy) do?
- [ ] Handles inbound traffic from the internet to your web server
- [ ] Takes user requests inside your network and forwards them out to the internet
- [ ] Acts as an uncontrolled third-party proxy
- [ ] Balances load across database servers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Takes user requests inside your network and forwards them out to the internet</p>
<p>Users send requests to the internal proxy server inside the network, which then forwards them out to the internet.</p>
</details>

---

### 13. What does a reverse proxy do?
- [ ] Forwards internal user requests out to the internet
- [ ] Receives inbound requests from the internet before they reach your internal web server, and can drop requests or cache responses
- [ ] Bypasses existing security controls
- [ ] Encrypts traffic between two sites

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Receives inbound requests from the internet before they reach your internal web server, and can drop requests or cache responses</p>
<p>Caching responses on the reverse proxy limits how much web traffic hits your web server.</p>
</details>

---

### 14. Why is an open proxy a security concern?
- [ ] It's always operated by your own IT team
- [ ] It's an uncontrolled third-party proxy, often used to circumvent security controls, and the third party could add ads or malicious code to traffic
- [ ] It only supports HTTPS
- [ ] It can't cache content

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's an uncontrolled third-party proxy, often used to circumvent security controls, and the third party could add ads or malicious code to traffic</p>
<p>Since you don't control an open proxy, you can't trust what it does to your traffic.</p>
</details>

---

### 15. Besides distributing the load across multiple servers, what other benefit does a load balancer provide?
- [ ] Fault tolerance — if one server fails, the load is split across the remaining servers
- [ ] It replaces the need for a firewall
- [ ] It authenticates wireless clients
- [ ] It stores encryption keys

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Fault tolerance — if one server fails, the load is split across the remaining servers</p>
<p>Load balancers are used in large-scale implementations like web server farms and database farms to keep the load even across devices.</p>
</details>

---

### 16. In active/active load balancing, what does SSL offload do?
- [ ] Removes all encryption from the network
- [ ] Performs encryption/decryption on the load balancer so the servers don't have to
- [ ] Keeps one TCP connection open all the time
- [ ] Sends traffic to a standby server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Performs encryption/decryption on the load balancer so the servers don't have to</p>
<p>Active/active load balancers can also provide TCP offloading (keeping one TCP connection open), caching for faster responses, and content switching for app-centric balancing.</p>
</details>

---

### 17. How does active/passive load balancing work?
- [ ] All servers are active at all times
- [ ] Some servers are active while others are on standby; if an active server fails, a passive server takes its place
- [ ] The load balancer itself is always passive
- [ ] Servers alternate being active every hour

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Some servers are active while others are on standby; if an active server fails, a passive server takes its place</p>
<p>In active/active, all connected servers are active. In active/passive, standby servers wait to take over.</p>
</details>

---

### 18. Which of these is an example of a collector rather than a sensor?
- [ ] Firewall logs
- [ ] Authentication logs
- [ ] A SIEM console or syslog server
- [ ] Email logs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A SIEM console or syslog server</p>
<p>Sensors (IPS, firewall logs, auth logs, email logs) are built into or attached to network devices. Collectors aggregate that info — proprietary consoles, SIEM consoles, and syslog servers. Most SIEMs include a correlation engine for data analysis.</p>
</details>

---

### 19. What is EAP?
- [ ] An encryption algorithm for VPNs
- [ ] The Extensible Authentication Protocol, an authentication framework with many different ways to authenticate based on RFC standards
- [ ] A type of load balancer
- [ ] A firewall rule format

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The Extensible Authentication Protocol, an authentication framework with many different ways to authenticate based on RFC standards</p>
<p>EAP integrates with 802.1X to prevent access to the network until authentication succeeds.</p>
</details>

---

### 20. What is IEEE 802.1X also known as?
- [ ] Port-based Network Access Control (NAC)
- [ ] Next-Generation Firewall
- [ ] Software Defined WAN
- [ ] Unified Threat Management

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Port-based Network Access Control (NAC)</p>
<p>With 802.1X, you can't access the network until you authenticate. It's used with an authentication database and is common on wireless networks, though it works on wired networks too.</p>
</details>

---

### 21. In 802.1X, what are the roles of the supplicant, authenticator, and authentication server?
- [ ] Supplicant = the client; authenticator = the device that provides access; authentication server = validates the client's credentials
- [ ] Supplicant = the switch; authenticator = the client; authentication server = the firewall
- [ ] Supplicant = the auth database; authenticator = the user; authentication server = the router
- [ ] All three are the same device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Supplicant = the client; authenticator = the device that provides access; authentication server = validates the client's credentials</p>
<p>The authenticator sends an EAP-request to the supplicant, the supplicant sends back an EAP-response, and the authentication server verifies it.</p>
</details>

---

### 22. A network-based firewall filtering by port number operates at which OSI layer, versus one filtering by specific application?
- [ ] Layer 2 vs. Layer 3
- [ ] Layer 4 (TCP/UDP) vs. Layer 7 (applications)
- [ ] Layer 1 vs. Layer 7
- [ ] Layer 3 vs. Layer 5

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Layer 4 (TCP/UDP) vs. Layer 7 (applications)</p>
<p>Network-based firewalls filter traffic by port number (layer 4) or application (layer 7). Many can also act as layer 3 devices (routers), often with NAT functionality and authenticated dynamic routing.</p>
</details>

---

### 23. What is the main drawback of a Unified Threat Management (UTM) device?
- [ ] It has only one feature
- [ ] Running all its combined features can reduce its performance
- [ ] It can't filter spam
- [ ] It doesn't include a firewall

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Running all its combined features can reduce its performance</p>
<p>A UTM is an all-in-one appliance: URL filtering/content inspection, malware inspection, spam filtering, CSU/DSU WAN connectivity, firewall, IDS/IPS, bandwidth shaping, and VPN endpoint.</p>
</details>

---

### 24. What does a Next-Generation Firewall (NGFW) let you do that a traditional port-based firewall can't?
- [ ] Only block traffic by IP address
- [ ] Control traffic flows based on the application, such as allowing users to view Twitter but not post
- [ ] Remove the need to analyze packets
- [ ] Operate only at OSI layer 2

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Control traffic flows based on the application, such as allowing users to view Twitter but not post</p>
<p>An NGFW is an OSI layer 7 firewall that must analyze and categorize every packet before making a security decision. It also includes IPS (identify the app and apply app-specific vulnerability signatures) and URL filtering by category.</p>
</details>

---

### 25. How does a Web Application Firewall (WAF) differ from a normal firewall?
- [ ] It only filters by port number
- [ ] It applies rules to HTTP/S conversations, allowing or denying based on expected input
- [ ] It only works for email traffic
- [ ] It replaces the need for VPNs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It applies rules to HTTP/S conversations, allowing or denying based on expected input</p>
<p>Unexpected input (like SQL injection) is a common way of exploiting an app. WAFs are a major focus of PCI DSS and are often used together with an NGFW.</p>
</details>

---

### 26. What is a VPN concentrator?
- [ ] A device that cools servers
- [ ] An encryption/decryption access device, often integrated into a firewall or available as software or built into the OS
- [ ] A type of load balancer
- [ ] A wireless access point

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An encryption/decryption access device, often integrated into a firewall or available as software or built into the OS</p>
<p>VPNs send encrypted data across a public network, and the concentrator handles the encryption and decryption.</p>
</details>

---

### 27. In an IPsec encrypted tunnel, how does the encrypted data still reach its destination?
- [ ] The original packet is sent unencrypted
- [ ] The original IP header and data are encrypted, then a new IP header (to the IPsec concentrator) plus an IPsec header and trailer are added; the concentrator decrypts and forwards the original traffic
- [ ] The packet is broadcast to every device on the network
- [ ] Only the data is encrypted and the original header is kept

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The original IP header and data are encrypted, then a new IP header (to the IPsec concentrator) plus an IPsec header and trailer are added; the concentrator decrypts and forwards the original traffic</p>
<p>Wrapping the encrypted packet in new headers keeps the data private while still routing it to the concentrator.</p>
</details>

---

### 28. Why do SSL/TLS VPNs usually have no firewall issues?
- [ ] They use the common TCP port 443
- [ ] They don't use any ports
- [ ] They require a dedicated hardware concentrator
- [ ] They only work on internal networks

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They use the common TCP port 443</p>
<p>SSL/TLS VPNs don't need big VPN clients (they can even run inside the browser), and they authenticate users without shared passwords or digital certificates.</p>
</details>

---

### 29. What describes a site-to-site IPsec VPN?
- [ ] It's always on, and firewalls often act as the VPN concentrators
- [ ] It only runs inside a web browser
- [ ] It must be manually connected by each user
- [ ] It uses TCP port 443 exclusively

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's always on, and firewalls often act as the VPN concentrators</p>
<p>Site-to-site IPsec VPNs permanently connect two networks, with the firewall at each site handling the tunnel.</p>
</details>

---

### 30. What problem does SD-WAN solve?
- [ ] It removes the need for encryption
- [ ] Remote sites no longer need to hop through a central data center to reach cloud-based apps; a dynamic network communicates with cloud services directly
- [ ] It replaces all firewalls with load balancers
- [ ] It forces all traffic through one data center

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Remote sites no longer need to hop through a central data center to reach cloud-based apps; a dynamic network communicates with cloud services directly</p>
<p>WAN connections used to go from every remote site to one data center, but databases and web services have moved into the cloud. Relaying through the data center adds an extra hop.</p>
</details>

---

### 31. What is Secure Access Service Edge (SASE)?
- [ ] A next-generation VPN with security technologies in the cloud close to cloud services, and SASE clients on all devices
- [ ] A type of on-premises load balancer
- [ ] A legacy dial-up access method
- [ ] A physical air-gapped network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A next-generation VPN with security technologies in the cloud close to cloud services, and SASE clients on all devices</p>
<p>SASE updates secure access for cloud services, letting any device securely connect to cloud services from different locations.</p>
</details>
