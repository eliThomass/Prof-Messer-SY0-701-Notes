# Quiz 4.5 — Firewalls
*Professor Messer SY0-701 · Section 4.5*

---

### 1. At which OSI layer does a next-generation firewall (NGFW) operate?
- [ ] Layer 2
- [ ] Layer 3
- [ ] Layer 4
- [ ] Layer 7

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Layer 7</p>
<p>An NGFW works at the OSI application layer. Every packet must be analyzed, categorized, and a decision determined, which requires some advanced decodes.</p>
</details>

---

### 2. Which of these is another name for an NGFW?
- [ ] Transparent proxy server
- [ ] Deep packet inspection device
- [ ] Screened subnet router
- [ ] Secure mail gateway device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Deep packet inspection device</p>
<p>An NGFW can also be called an application layer gateway or a stateful multilayer inspection device.</p>
</details>

---

### 3. Besides filtering traffic, what else can a network-based firewall provide?
- [ ] File integrity monitoring and USB blocking
- [ ] Email validation and DKIM signing
- [ ] Site-to-site VPN encryption, NAT, and dynamic routing
- [ ] Posture assessments and user behavior analytics

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Site-to-site VPN encryption, NAT, and dynamic routing</p>
<p>Most firewalls can act as layer 3 devices and often sit on the ingress/egress of the network.</p>
</details>

---

### 4. What does a traditional port-based firewall use to make forwarding decisions?
- [ ] The application running inside the traffic
- [ ] The protocol and port number
- [ ] The user's Active Directory group
- [ ] The website's reputation score

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The protocol and port number</p>
<p>Examples are tcp/443 for HTTPS and udp/53 for DNS. NGFWs can use these too, as additional security policy options.</p>
</details>

---

### 5. Firewall rules are usually evaluated top-to-bottom. Where should the more specific rules go?
- [ ] At the top of the rule list
- [ ] At the bottom of the rule list
- [ ] In the middle of the rule list
- [ ] In a separate rule list

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> At the top of the rule list</p>
<p>Rules follow a logical path, so specific rules go first and more generic rules sit lower in the list.</p>
</details>

---

### 6. Traffic reaches a firewall and doesn't match any rule in the list. What does an implicit deny do?
- [ ] Forwards the traffic to the screened subnet
- [ ] Allows the traffic and sends an alert
- [ ] Sends the traffic back through the rule list
- [ ] Blocks the traffic

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Blocks the traffic</p>
<p>An implicit deny is a deny at the bottom of the rule list that catches any traffic no other rule matched.</p>
</details>

---

### 7. Which of these would you find in a firewall access control list (ACL)?
- [ ] Source IP, destination IP, and port number
- [ ] Password age and expiration
- [ ] CVSS score and CVE number
- [ ] Asset tag and tracking number

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Source IP, destination IP, and port number</p>
<p>An ACL allows or disallows traffic based on groupings of categories like these.</p>
</details>

---

### 8. A company hosts a public web server but doesn't want Internet users reaching its internal network. Where should the server go?
- [ ] On the internal network, behind a NAT
- [ ] On a user's workstation
- [ ] In a screened subnet
- [ ] Behind a forward proxy

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> In a screened subnet</p>
<p>A screened subnet is an extra layer of security between you and the Internet. It holds services that must be reachable from the Internet, and that traffic is redirected there instead of the internal network.</p>
</details>

---

### 9. Which IPS detection method looks for a perfect match against known patterns?
- [ ] Anomaly-based
- [ ] Reputation-based
- [ ] Behavior-based
- [ ] Signature-based

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Signature-based</p>
<p>An IPS usually has thousands of signatures inside, and the rules can be customized by group. IPS is usually integrated into an NGFW.</p>
</details>

---

### 10. How does anomaly-based IPS detection work?
- [ ] It compares files against a list of known hashes
- [ ] It builds a baseline of what's normal and flags unusual traffic patterns
- [ ] It blocks every website outside an allow list
- [ ] It matches traffic against a signature database

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It builds a baseline of what's normal and flags unusual traffic patterns</p>
<p>Whichever detection method is used, you determine what happens when unwanted traffic appears: block it, allow it, send an alert, and so on.</p>
</details>

---

### 11. What is content filtering based on?
- [ ] The source port of the connection
- [ ] The MAC address of the device
- [ ] The data within the content
- [ ] The time of day

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The data within the content</p>
<p>Content filtering gives corporate control of inbound and outbound data, controls inappropriate content, and protects against malicious websites.</p>
</details>

---

### 12. What is a limitation of URL scanning?
- [ ] It can't be integrated into an NGFW
- [ ] It can only use a block list, not an allow list
- [ ] URLs can't be managed by category
- [ ] Control is limited, because URLs aren't the only way to surf

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Control is limited, because URLs aren't the only way to surf</p>
<p>URL scanning allows or restricts traffic by URL, using allow lists, block lists, and categories like auction, hacking, and malware.</p>
</details>

---

### 13. Where does the filtering decision happen with an agent-based content filter?
- [ ] On the user's device
- [ ] On the corporate firewall
- [ ] On a proxy in the data center
- [ ] On the DNS server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> On the user's device</p>
<p>The client software is managed from a central console, so users can be anywhere and are always filtered. Updates must be distributed to all agents, often from the cloud.</p>
</details>

---

### 14. What does a proxy do?
- [ ] Encrypts every file on the user's device
- [ ] Signs all outgoing email
- [ ] Receives user requests and sends them on the user's behalf
- [ ] Assigns IP addresses to devices on the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Receives user requests and sends them on the user's behalf</p>
<p>A proxy sits between the users and the external network, which lets you control the flow of traffic. It's also useful for caching and access control.</p>
</details>

---

### 15. What is the difference between an explicit proxy and a transparent proxy?
- [ ] Explicit proxies cache data; transparent proxies don't
- [ ] Applications must be configured for an explicit proxy, while a transparent proxy is invisible to them
- [ ] Explicit proxies only handle inbound traffic; transparent proxies only handle outbound traffic
- [ ] Transparent proxies must be installed on each device; explicit proxies don't need installing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Applications must be configured for an explicit proxy, while a transparent proxy is invisible to them</p>
<p>With an explicit proxy, the app needs to know how to use it.</p>
</details>

---

### 16. A content filter is set to "Gambling: Block" and "Home and Garden: Allow and Alert." What are "Block" and "Allow and Alert" examples of?
- [ ] Dispositions
- [ ] Signatures
- [ ] Reputations
- [ ] Rules of engagement

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Dispositions</p>
<p>Block rules can be based on a specific URL or a site category, and categories are usually divided into over 50 topics. Each one gets a disposition.</p>
</details>

---

### 17. A content filter scans a site and assigns it a risk level automatically. What is this called?
- [ ] DNS filtering
- [ ] URL scanning
- [ ] Automated reputation
- [ ] Manual reputation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Automated reputation</p>
<p>Reputation filtering works off perceived risk, from trustworthy through low, medium, and high risk to suspicious. With manual reputation, managers set the reputation themselves.</p>
</details>

---

### 18. How does DNS filtering stop a user from reaching a harmful site?
- [ ] It inspects the page after it loads
- [ ] It quarantines the user's device
- [ ] It installs an agent on the user's device
- [ ] The DNS server doesn't resolve the harmful site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The DNS server doesn't resolve the harmful site</p>
<p>DNS is updated with real-time threat intelligence. Because it applies to any DNS lookup, it works for more than just web filtering.</p>
</details>

---

### 19. Which best describes Active Directory?
- [ ] A Windows-based database of everything on the network
- [ ] A Linux kernel patch that adds mandatory access control
- [ ] A tool that monitors important files for changes
- [ ] A protocol for encrypting network traffic between sites

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A Windows-based database of everything on the network</p>
<p>It holds computers, user accounts, file shares, printers, and groups. Users log in with their AD credentials, it acts as a centralized access control list, and the help desk commonly uses it for passwords and adding or removing accounts.</p>
</details>

---

### 20. An admin wants to push login scripts and security settings to computers across a Windows domain. Which console should they use?
- [ ] Security console
- [ ] System File Checker
- [ ] Group Policy Management Editor
- [ ] Central agent console

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Group Policy Management Editor</p>
<p>Group Policy manages computers or users with local and domain policies, offering hundreds of config options like login scripts, network configs, and security parameters.</p>
</details>

---

### 21. What does SELinux add to the Linux kernel?
- [ ] Discretionary access control (DAC)
- [ ] Group Policy
- [ ] Active Directory integration
- [ ] Mandatory access control (MAC)

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Mandatory access control (MAC)</p>
<p>Linux traditionally uses DAC. SELinux limits application access using least privilege, so a potential breach has limited scope.</p>
</details>

---

### 22. Which group contains only unencrypted protocols?
- [ ] Telnet, FTP, SMTP, IMAP
- [ ] HTTPS, Telnet, FTP, SMTP
- [ ] WPA3, Telnet, IMAP, FTP
- [ ] HTTPS, WPA3, VPN, DKIM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Telnet, FTP, SMTP, IMAP</p>
<p>You can verify whether traffic is encrypted with a packet capture.</p>
</details>

---

### 23. An application runs on port 443. Does that prove the connection is secure?
- [ ] Yes, port 443 is always HTTPS
- [ ] No, the port number does not guarantee security
- [ ] Yes, firewalls block insecure traffic on port 443
- [ ] Only if the application also uses port 80

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> No, the port number does not guarantee security</p>
<p>Secure and insecure connections often run on different ports, like 80 for HTTP and 443 for HTTPS, but the port alone isn't proof.</p>
</details>

---

### 24. An application doesn't offer a secure protocol. Which approach encrypts its traffic anyway?
- [ ] Moving it to a different port number
- [ ] Adding a firewall rule at the bottom of the list
- [ ] Sending it through a VPN's encrypted tunnel
- [ ] Connecting over an open access point

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Sending it through a VPN's encrypted tunnel</p>
<p>This is the transport method approach: don't rely on the application, encrypt everything. On 802.11 wireless, WPA3 also encrypts all user data, while an open access point has no transport-level encryption.</p>
</details>

---

### 25. What is the role of a mail gateway?
- [ ] It evaluates inbound email and blocks bad messages before they reach users
- [ ] It stores all of a user's passwords in an encrypted database
- [ ] It publishes the organization's DKIM keys to every user's mail client
- [ ] It checks every device's patch level before it joins the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It evaluates inbound email and blocks bad messages before they reach users</p>
<p>A mail gateway is the gatekeeper of all mail for an organization, and it can be on-site or cloud-based. It matters because email protocols have few security checks, which makes spoofing easy.</p>
</details>

---

### 26. Which email security method lists all the servers authorized to send mail for a domain?
- [ ] DKIM
- [ ] DMARC
- [ ] SMTP
- [ ] SPF

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> SPF</p>
<p>Sender Policy Framework answers "who can send mail on your behalf?" Receiving mail servers check whether incoming mail came from an authorized host.</p>
</details>

---

### 27. How does DKIM validate email?
- [ ] The sending server signs outgoing mail, and receiving servers validate the signature
- [ ] The receiving server checks the sender's IP against a list of authorized hosts
- [ ] The end user checks each message's signature before opening it in their client
- [ ] The mail gateway encrypts the message body separately for each recipient

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The sending server signs outgoing mail, and receiving servers validate the signature</p>
<p>DKIM stands for Domain Keys Identified Mail. The public key is in a DNS TXT record, and the signature usually isn't seen by the end user.</p>
</details>

---

### 28. A domain owner wants receiving mail servers to reject any email that fails SPF and DKIM. Which method sets that policy?
- [ ] FIM
- [ ] DMARC
- [ ] DLP
- [ ] SAML

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> DMARC</p>
<p>The domain owner writes the policy into a DNS TXT record, such as accept all, send to spam, or reject all.</p>
</details>

---

### 29. Besides setting a policy, what else does DMARC give the domain owner?
- [ ] Compliance reports on validation statistics
- [ ] A digital signature on each outgoing message
- [ ] A list of every authorized mail server
- [ ] Automatic encryption of all email in transit

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Compliance reports on validation statistics</p>
<p>The reports are sent to the email administrator and can reveal if someone is spoofing the domain.</p>
</details>

---

### 30. Which tools perform file integrity monitoring on Windows and Linux?
- [ ] Group Policy on Windows, SELinux on Linux
- [ ] Active Directory on Windows, LDAP on Linux
- [ ] System File Checker on Windows, Tripwire on Linux
- [ ] Tripwire on Windows, System File Checker on Linux

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> System File Checker on Windows, Tripwire on Linux</p>
<p>Some files should never change, so FIM monitors important OS and application files and identifies when changes occur. Many host-based IPS options do this too.</p>
</details>

---

### 31. Match the DLP location to the data state. Which pairing is correct?
- [ ] Endpoint: data in use, network: data in motion, server: data at rest
- [ ] Endpoint: data at rest, network: data in use, server: data in motion
- [ ] Endpoint: data in motion, network: data at rest, server: data in use
- [ ] Endpoint: data in use, network: data at rest, server: data in motion

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Endpoint: data in use, network: data in motion, server: data at rest</p>
<p>DLP blocks sensitive data in real time and often needs multiple solutions. Endpoint DLP usually watches your RAM.</p>
</details>

---

### 32. What did the November 2008 US Department of Defense incident lead to?
- [ ] A ban on all email attachments across the DoD
- [ ] A department-wide move to cloud-based DLP
- [ ] Mandatory use of SELinux on all workstations
- [ ] A local DLP agent that blocked all USB connections

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A local DLP agent that blocked all USB connections</p>
<p>The DoD was infiltrated through USB storage. DLP on a workstation can allow or deny tasks like this.</p>
</details>

---

### 33. Where does cloud-based DLP sit?
- [ ] On each user's workstation
- [ ] Between users and the Internet
- [ ] Inside the mail server
- [ ] On the storage drives in the data center

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Between users and the Internet</p>
<p>From there it watches every byte of network traffic, blocks custom defined data strings and malware, and manages URL access to prevent file transfers to the cloud.</p>
</details>

---

### 34. Which is an example of outbound email DLP?
- [ ] Identifying imposters in received messages
- [ ] Quarantining suspicious incoming messages
- [ ] Stopping fake wire transfers and W-2 transmissions
- [ ] Blocking keywords in messages from outside senders

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Stopping fake wire transfers and W-2 transmissions</p>
<p>Email is still the most critical risk vector, so every message is checked in both directions. The other three options are inbound checks.</p>
</details>

---

### 35. How does control at the edge compare to access control?
- [ ] Edge firewall rules rarely change, while access control can be easily revoked or changed by user, group, location, or app
- [ ] Edge firewall rules change constantly, while access control never changes
- [ ] Edge control is based on user and group, while access control is based on port number
- [ ] Both are managed entirely through firewall rules on the Internet link

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Edge firewall rules rarely change, while access control can be easily revoked or changed by user, group, location, or app</p>
<p>Control at the edge happens at your Internet link. Access control can be managed from wherever you are.</p>
</details>

---

### 36. When is the best time to perform a posture assessment?
- [ ] Once a year during an audit
- [ ] After a breach is detected
- [ ] When the device is decommissioned
- [ ] When the device first connects to the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> When the device first connects to the network</p>
<p>You can't trust everyone's computer, so posture assessments look for anything not up to the latest security standards, like app versions and anti-virus.</p>
</details>

---

### 37. Which agent type needs no install, runs during the posture assessment, and then removes itself?
- [ ] Dissolvable agent
- [ ] Persistent agent
- [ ] Agentless NAC
- [ ] Lightweight EDR agent

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Dissolvable agent</p>
<p>A persistent agent, by contrast, is permanently installed and monitors all apps for the assessment.</p>
</details>

---

### 38. What is true of agentless NAC?
- [ ] It's permanently installed on each system and monitors all apps
- [ ] It's integrated with Active Directory, with checks made during login and logoff
- [ ] It can be scheduled to run at any time of day or night
- [ ] It runs from removable media that removes itself afterward

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's integrated with Active Directory, with checks made during login and logoff</p>
<p>Because the checks are tied to login and logoff, agentless NAC can't be scheduled.</p>
</details>

---

### 39. A device fails its posture assessment. What typically happens next?
- [ ] It's physically destroyed and replaced with a new compliant device
- [ ] Its user account is deleted and must be provisioned again
- [ ] It's quarantined on its own VLAN until the issue is resolved, then tried again
- [ ] It's allowed onto the network and the security team gets an alert

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's quarantined on its own VLAN until the issue is resolved, then tried again</p>
<p>Quarantine keeps the device away from the rest of the network while it's being fixed.</p>
</details>

---

### 40. How does EDR detect threats differently from signature-only tools?
- [ ] It relies on a much larger and more frequently updated signature database
- [ ] It only scans files once a day, outside of normal working hours
- [ ] It requires a user to review and approve each detection
- [ ] It also uses behavioral analysis, machine learning, and process monitoring

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It also uses behavioral analysis, machine learning, and process monitoring</p>
<p>EDR uses a lightweight agent on the endpoint to detect a threat, then investigates it with root cause analysis.</p>
</details>

---

### 41. Which of these is an EDR response to a threat?
- [ ] Publishing a DMARC policy that rejects the attacker's messages
- [ ] Isolating the system, quarantining the threat, or rolling back to a previous config
- [ ] Assigning the threat a CVE number and a CVSS score
- [ ] Waiting for a user to submit a ticket, then scheduling a manual fix

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Isolating the system, quarantining the threat, or rolling back to a previous config</p>
<p>The response is API driven, so no user intervention is required.</p>
</details>

---

### 42. What does XDR add on top of EDR?
- [ ] Network-based detection and correlation of endpoint, network, and cloud data
- [ ] A single agent that watches one endpoint with more detailed signatures
- [ ] A replacement for all network firewalls and IPS devices
- [ ] Physical security monitoring for the data center and office spaces

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network-based detection and correlation of endpoint, network, and cloud data</p>
<p>Attacks involve more than the endpoint. XDR evolves EDR by improving missed detections, false positives, and long investigation times.</p>
</details>

---

### 43. What does user behavior analytics need before it can flag unusual activity?
- [ ] A signed certificate issued to each user and each host
- [ ] A baseline of normal activity, built over an extended period
- [ ] A dissolvable agent installed on every device in the org
- [ ] A list of every authorized application and mail server

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A baseline of normal activity, built over an extended period</p>
<p>XDR commonly includes this. It watches users, hosts, network traffic, and data repositories, then uses rulesets, pattern matching, and statistical analysis to spot anything unusual.</p>
</details>
