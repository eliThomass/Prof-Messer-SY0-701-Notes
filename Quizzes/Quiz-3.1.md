# Quiz 3.1 — Cloud Infrastructure
*Professor Messer SY0-701 · Section 3.1*

---

### 1. In IaaS, PaaS, and SaaS models, how do you find out who is responsible for each part of security?
- [ ] The customer is always responsible for everything
- [ ] The cloud provider documents it in a responsibility matrix, which can vary between providers
- [ ] The provider is always responsible for everything
- [ ] It's decided after a breach occurs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The cloud provider documents it in a responsibility matrix, which can vary between providers</p>
<p>Security responsibilities should be well documented by the cloud provider in a matrix of responsibilities that splits duties between the provider and the customer.</p>
</details>

---

### 2. What is a hybrid cloud?
- [ ] A cloud that runs only on-premises
- [ ] More than one public or private cloud used together
- [ ] A cloud with no security controls
- [ ] A single public cloud with multiple users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> More than one public or private cloud used together</p>
<p>A hybrid cloud adds complexity: network protection mismatches, authentication across platforms, separate firewall configs per provider, diverse cloud-specific logs, and data leakage across the public internet.</p>
</details>

---

### 3. Which of these is a security concern specific to hybrid clouds?
- [ ] Network protection mismatches, because cloud providers work in different ways
- [ ] There's only one set of logs to review
- [ ] All providers share the same firewall configuration
- [ ] Data never crosses the public internet

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network protection mismatches, because cloud providers work in different ways</p>
<p>Each provider needs its own firewall configs, authentication, and matching server settings, and security monitoring differs since logs are diverse and cloud-specific.</p>
</details>

---

### 4. How should third-party vendors in the cloud be managed?
- [ ] Assess them once during onboarding and never again
- [ ] Ongoing vendor risk assessments, including them in incident response, and constant monitoring
- [ ] Leave them out of incident response entirely
- [ ] Give them full admin access to simplify things

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Ongoing vendor risk assessments, including them in incident response, and constant monitoring</p>
<p>Vendor risk assessments are part of an overall vendor risk management policy. Third-party impact should be included in incident response, since everyone is part of the process.</p>
</details>

---

### 5. What is the main benefit of Infrastructure as Code (IaC)?
- [ ] It removes the need for servers
- [ ] Infrastructure is described as code, so it can be versioned and built the same way every time
- [ ] It only works on physical hardware
- [ ] It eliminates the need for networking

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Infrastructure is described as code, so it can be versioned and built the same way every time</p>
<p>IaC describes servers, networks, and apps as code, making infrastructure easier to change and version. That same code can build other app instances, producing a perfect version each time.</p>
</details>

---

### 6. What is serverless architecture also known as?
- [ ] Infrastructure as a Service (IaaS)
- [ ] Function as a Service (FaaS)
- [ ] Software Defined Networking (SDN)
- [ ] Platform as a Service (PaaS)

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Function as a Service (FaaS)</p>
<p>In serverless architecture, apps are separated into individual, autonomous functions, which removes the OS from the equation.</p>
</details>

---

### 7. In a serverless architecture, who handles the operating system's security concerns?
- [ ] The developer
- [ ] The end user
- [ ] The third party managing the platform
- [ ] No one, since there is no OS

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The third party managing the platform</p>
<p>The developer still writes the server-side logic, which runs in a stateless compute container that may be event-triggered and ephemeral. The platform is managed by a third party, so all OS security concerns fall on them.</p>
</details>

---

### 8. What is the role of APIs in a microservices architecture?
- [ ] They replace the need for any code
- [ ] They're the glue that lets microservices work together as the application, making it scalable, resilient, and secure
- [ ] They combine everything into one monolithic app
- [ ] They're only used for logging

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They're the glue that lets microservices work together as the application, making it scalable, resilient, and secure</p>
<p>Unlike a monolithic app, which contains all the decision-making in one large codebase, microservices connected by APIs keep outages contained.</p>
</details>

---

### 9. Placing web servers in one rack and database servers in another rack with an air gap between them is an example of what?
- [ ] Logical segmentation with VLANs
- [ ] Physical isolation
- [ ] Software Defined Networking
- [ ] Containerization

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Physical isolation</p>
<p>Physically isolated devices have an air gap between them and must be physically connected to communicate. Another example is putting Customer A on one switch and Customer B on a different switch.</p>
</details>

---

### 10. How do VLANs differ from physical isolation?
- [ ] VLANs separate switches logically instead of physically
- [ ] VLANs require a separate switch for every customer
- [ ] VLANs create an air gap between devices
- [ ] VLANs only work in the cloud

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> VLANs separate switches logically instead of physically</p>
<p>Logical segmentation with VLANs separates networks on the same hardware without needing physically separate switches.</p>
</details>

---

### 11. In Software Defined Networking (SDN), which plane processes network frames and packets, handling forwarding, trunking, encrypting, and NAT?
- [ ] Control plane
- [ ] Management plane
- [ ] Data plane
- [ ] Application plane

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data plane</p>
<p>SDN splits a networking device's functions into separate logical units: the data, control, and management planes.</p>
</details>

---

### 12. Which SDN plane manages the actions of the data plane using routing tables, session tables, NAT tables, and dynamic routing protocol updates?
- [ ] Data plane
- [ ] Control plane
- [ ] Management plane
- [ ] Physical plane

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Control plane</p>
<p>The control plane manages the actions of the data plane.</p>
</details>

---

### 13. Which SDN plane is used to configure and manage the device through SSH, a browser, or an API?
- [ ] Data plane
- [ ] Control plane
- [ ] Management plane
- [ ] Forwarding plane

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Management plane</p>
<p>The management plane is where administrators configure and manage the device.</p>
</details>

---

### 14. What is an advantage of cloud-based security compared to on-premises security?
- [ ] The client carries the entire security burden
- [ ] It's centralized and costs less, with no dedicated hardware or data center to secure
- [ ] You get full control to customize everything
- [ ] Security changes always take longer

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's centralized and costs less, with no dedicated hardware or data center to secure</p>
<p>On-premises puts the security burden on the client. Attacks can happen anywhere, so there are arguments for both approaches.</p>
</details>

---

### 15. What is an advantage of on-premises security?
- [ ] Security changes are always instant
- [ ] Full control to customize your security posture, with an on-site IT team managing security and uptime
- [ ] No hardware to maintain
- [ ] The provider handles all security

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Full control to customize your security posture, with an on-site IT team managing security and uptime</p>
<p>On-premises gives full control, and a local team maintains uptime and availability. The downside is that security changes can take time.</p>
</details>

---

### 16. What is the main drawback of a centralized security approach?
- [ ] It can't correlate alerts
- [ ] It's a single point of failure
- [ ] It can't consolidate log files
- [ ] It gives no view of system status

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's a single point of failure</p>
<p>Most organizations are physically decentralized and hard to protect. A centralized approach provides correlated alerts, consolidated log analysis, and comprehensive system status, but it's not perfect since it's a single point of failure.</p>
</details>

---

### 17. How does virtualization differ from application containerization?
- [ ] In virtualization, each app instance has its own OS on a hypervisor; containers share the host kernel and only need an OS to run on
- [ ] Containers each run their own full operating system
- [ ] Virtualization doesn't use a hypervisor
- [ ] They are exactly the same

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> In virtualization, each app instance has its own OS on a hypervisor; containers share the host kernel and only need an OS to run on</p>
<p>Virtualization stacks as infrastructure, then hypervisor, then VMs with their own OSes and apps. A container holds the code and dependencies needed to run an app, and a container image is a lightweight, portable standard that uses the host kernel.</p>
</details>

---

### 18. Why can't containers interact with each other by default?
- [ ] Each is an isolated, self-contained process (a sandbox)
- [ ] They run on separate physical servers
- [ ] They each have their own hypervisor
- [ ] They're always air-gapped

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Each is an isolated, self-contained process (a sandbox)</p>
<p>A container is a standardized unit of software, and each container runs as an isolated process that can't interact with others.</p>
</details>

---

### 19. What is SCADA (also known as ICS) used for?
- [ ] Hosting websites in the cloud
- [ ] Managing industrial equipment like power generation, refining, and manufacturing, with real-time info and system control
- [ ] Running microservices with APIs
- [ ] Encrypting files on a laptop

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Managing industrial equipment like power generation, refining, and manufacturing, with real-time info and system control</p>
<p>Supervisory Control and Data Acquisition (SCADA) systems, also called Industrial Control Systems (ICS), require extensive segmentation and no outside access. They're some of the most secure systems in the world.</p>
</details>

---

### 20. What defines a Real-Time Operating System (RTOS)?
- [ ] It only runs at night
- [ ] It has a deterministic processing schedule with no time to wait for other processes
- [ ] It's always cloud-hosted
- [ ] It doesn't need to always be available

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It has a deterministic processing schedule with no time to wait for other processes</p>
<p>An RTOS is used in industrial equipment, automobiles, and military environments. These systems are extremely sensitive to security issues because they need to always be available.</p>
</details>

---

### 21. Traffic light controllers, digital watches, and medical imaging systems are examples of what?
- [ ] Embedded systems
- [ ] Serverless functions
- [ ] Hybrid clouds
- [ ] Container images

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Embedded systems</p>
<p>Embedded systems are hardware and software designed for one specific purpose.</p>
</details>

---

### 22. What is the difference between redundancy and high availability (HA)?
- [ ] There is no difference
- [ ] Redundancy doesn't always mean always available (a backup may need to be powered on manually), while HA means always on, always available
- [ ] HA systems are always powered off until needed
- [ ] Redundancy guarantees zero downtime

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Redundancy doesn't always mean always available (a backup may need to be powered on manually), while HA means always on, always available</p>
<p>HA may include many components working together, and an active/active setup can provide scalability advantages.</p>
</details>

---

### 23. Why is availability described as a balancing act with security?
- [ ] Systems should be available, but only to the right people
- [ ] Availability always means no security
- [ ] Secure systems can never be available
- [ ] Availability doesn't cost anything

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Systems should be available, but only to the right people</p>
<p>Availability (system uptime) is an important metric — organizations are often evaluated on total available time, like 99% uptime — and lots of money is spent on it.</p>
</details>

---

### 24. What metric is commonly used to describe resilience?
- [ ] MTTR (Mean Time To Repair)
- [ ] RTOS
- [ ] FaaS
- [ ] SCADA

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> MTTR (Mean Time To Repair)</p>
<p>Resilience is about whether you can maintain availability and recover quickly when something goes down. It depends on variables like the root cause, replacement hardware, and software patches.</p>
</details>

---

### 25. The ability to quickly and easily increase or decrease capacity is known as what?
- [ ] Responsiveness
- [ ] Elasticity
- [ ] Resilience
- [ ] Risk transference

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Elasticity</p>
<p>Scalability is measured by elasticity. Security monitoring must also scale up and down along with the system.</p>
</details>

---

### 26. Buying cybersecurity insurance to recover losses during downtime and help with legal costs is an example of what?
- [ ] Risk transference
- [ ] Ease of recovery
- [ ] Patch availability
- [ ] Elasticity

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Risk transference</p>
<p>Risk transference minimizes risk by transferring it to a third party. Cybersecurity insurance recovers internal losses from attack downtime and protects against legal issues from customers.</p>
</details>

---

### 27. What is the recommended approach for embedded systems that can't be patched?
- [ ] Ignore the risk
- [ ] Add security controls around the device, like a firewall
- [ ] Have end users update them manually
- [ ] Unplug them permanently

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Add security controls around the device, like a firewall</p>
<p>Embedded systems often aren't designed for end-user updates, so additional security controls are placed around them.</p>
</details>

---

### 28. Which of the following are backup power services?
- [ ] UPS (uninterruptible power supply) and generators
- [ ] VLANs and SDN
- [ ] SIEM and EDR
- [ ] FaaS and IaaS

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> UPS (uninterruptible power supply) and generators</p>
<p>Most organizations rely on a primary power provider, with UPS units and generators as backup. A licensed electrician should handle power usage and extensions.</p>
</details>

---

### 29. In cloud terms, what is the "compute engine"?
- [ ] The part that handles an app's heavy lifting, from a single processor to multiple CPUs across clouds
- [ ] The backup power system
- [ ] The management plane of SDN
- [ ] A type of container image

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The part that handles an app's heavy lifting, from a single processor to multiple CPUs across clouds</p>
<p>Compute can be spread across multiple CPUs and clouds for enhanced scalability.</p>
</details>
