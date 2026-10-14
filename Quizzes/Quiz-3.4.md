# Quiz 3.4 — Resiliency
*Professor Messer SY0-701 · Section 3.4*

---

### 1. What is a downside of High Availability (HA) compared to simple redundancy?
- [ ] HA systems must be powered on manually
- [ ] HA means higher costs, since many components work together to stay always on
- [ ] HA systems are never available
- [ ] HA can't use more than one component

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> HA means higher costs, since many components work together to stay always on</p>
<p>Redundancy doesn't always mean always available — a backup might need to be powered on manually. HA means always on, always available, but it costs more.</p>
</details>

---

### 2. What is server clustering?
- [ ] Spreading load across servers that are unaware of each other
- [ ] Combining two or more servers to operate as one large server, so users only see one device
- [ ] Placing servers in separate buildings
- [ ] Taking a snapshot of a server every 24 hours

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Combining two or more servers to operate as one large server, so users only see one device</p>
<p>Clustering easily increases capacity and availability, and the servers are usually configured with the same operating system.</p>
</details>

---

### 3. How does load balancing differ from server clustering?
- [ ] In load balancing, the servers are unaware of each other; in clustering, they work together as one server
- [ ] Load balancing requires all servers to run the same OS
- [ ] Clustering servers are unaware of each other
- [ ] There's no difference

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> In load balancing, the servers are unaware of each other; in clustering, they work together as one server</p>
<p>A load balancer distributes the load across individual devices, and it adds or removes devices to increase capacity or when a server stops working.</p>
</details>

---

### 4. What is the correct order of the site resiliency process?
- [ ] A disaster is called → recovery site is prepped → revert to primary → problem is addressed
- [ ] Recovery site is prepped → a disaster is called → problem is addressed → revert back to the primary location
- [ ] Problem is addressed → disaster is called → recovery site is prepped → revert to primary
- [ ] Revert to primary → recovery site is prepped → disaster is called → problem is addressed

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Recovery site is prepped → a disaster is called → problem is addressed → revert back to the primary location</p>
<p>The recovery site is ready ahead of time, so operations can move there when a disaster is declared and come back once the problem is fixed.</p>
</details>

---

### 5. Which type of recovery site is an exact replica of your data center, with constantly updated hardware, apps, and software?
- [ ] Cold site
- [ ] Warm site
- [ ] Hot site
- [ ] Geographic site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Hot site</p>
<p>With a hot site, you can flip a switch and everything moves over, so the service is fully back up even if the main data center is destroyed.</p>
</details>

---

### 6. What describes a cold site?
- [ ] An exact replica with all hardware ready to go
- [ ] An empty building with no hardware, no data, and no people — you bring everything with you
- [ ] A site with some equipment already in place
- [ ] A cloud-only backup

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An empty building with no hardware, no data, and no people — you bring everything with you</p>
<p>A cold site requires you to bring in your own data and bus in your team.</p>
</details>

---

### 7. A recovery site that has some equipment on hand, but isn't a full replica, is called what?
- [ ] Hot site
- [ ] Warm site
- [ ] Cold site
- [ ] Clustered site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Warm site</p>
<p>A warm site falls between a hot site and a cold site, with some equipment already at the secondary site.</p>
</details>

---

### 8. Why should recovery sites be geographically dispersed?
- [ ] To be physically different from the organization's primary location, so the same disaster doesn't affect both
- [ ] To make transporting equipment easier
- [ ] To keep everything in one building
- [ ] Because it's cheaper than a single site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To be physically different from the organization's primary location, so the same disaster doesn't affect both</p>
<p>Geographic dispersion can be a logistical challenge, such as transporting equipment and employees, and everything eventually needs to come back to the main site.</p>
</details>

---

### 9. What is the security benefit of platform diversity?
- [ ] It makes systems easier to manage
- [ ] Many vulnerabilities are specific to a single OS, so using different platforms limits the impact of any one vulnerability
- [ ] It eliminates all vulnerabilities
- [ ] It removes the need for patching

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Many vulnerabilities are specific to a single OS, so using different platforms limits the impact of any one vulnerability</p>
<p>Every OS has potential security issues. The trade-off is that using many different platforms is harder to manage.</p>
</details>

---

### 10. What is the purpose of a multi-cloud system?
- [ ] To plan for cloud outages by dispersing data both geographically and across cloud services
- [ ] To use only one cloud provider for simplicity
- [ ] To avoid the need for backups
- [ ] To keep all data on-premises

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To plan for cloud outages by dispersing data both geographically and across cloud services</p>
<p>Multi-cloud systems help you plan for every contingency.</p>
</details>

---

### 11. What must a Continuity of Operations Plan (COOP) include?
- [ ] Only more technology
- [ ] Alternatives to technology, like manual transactions, paper receipts, and phone calls for approvals, documented and tested before a problem occurs
- [ ] A plan written after the disaster
- [ ] Only cloud-based backups

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Alternatives to technology, like manual transactions, paper receipts, and phone calls for approvals, documented and tested before a problem occurs</p>
<p>COOP is the fallback method when disasters disrupt normal operations.</p>
</details>

---

### 12. What are the consequences of poor capacity planning?
- [ ] Too much demand causes app slowdowns and outages; too much supply means overspending
- [ ] Too much supply causes outages
- [ ] Too much demand saves money
- [ ] There are no consequences

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Too much demand causes app slowdowns and outages; too much supply means overspending</p>
<p>Capacity planning matches supply to demand with a balanced approach: the right infrastructure, appropriate technology, and the appropriate number of people.</p>
</details>

---

### 13. In capacity planning for people, what should an organization do if it has too many employees for a service?
- [ ] Recruit more staff
- [ ] Redeploy them to other parts of the organization
- [ ] Shut down the service
- [ ] Move them all to the call center

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Redeploy them to other parts of the organization</p>
<p>Some services, like tech services and call center support lines, require human intervention. Too few employees means recruiting new staff.</p>
</details>

---

### 14. How can database services be scaled for capacity?
- [ ] Use a single SQL server only
- [ ] Have multiple SQL servers that can be enabled, and split the database to increase capacity
- [ ] Remove indexes from the database
- [ ] Move the database to a cold site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Have multiple SQL servers that can be enabled, and split the database to increase capacity</p>
<p>Pick a technology that can scale. Web services should use load balancers and servers, and cloud services offer seemingly unlimited resources on demand (for enough money).</p>
</details>

---

### 15. Why are cloud-based infrastructure devices easier for capacity planning than physical devices?
- [ ] Physical devices don't need to be configured
- [ ] Physical devices must be purchased, configured, and installed, while cloud-based devices are easier to deploy
- [ ] Cloud devices don't use CPU, network, or storage
- [ ] Cloud devices can't scale

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Physical devices must be purchased, configured, and installed, while cloud-based devices are easier to deploy</p>
<p>Infrastructure is the underlying framework — app servers, network services, CPU, network, and storage.</p>
</details>

---

### 16. Which of the following is a rule of engagement for recovery testing?
- [ ] Always test on the production systems
- [ ] Don't touch the production systems, and use a very specific scenario with limited time
- [ ] Test only after a real disaster happens
- [ ] Don't document the results

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Don't touch the production systems, and use a very specific scenario with limited time</p>
<p>Test yourself before an actual event, then evaluate the response, document it, and discuss it.</p>
</details>

---

### 17. What is a tabletop exercise?
- [ ] A full-scale simulated disaster that shuts down production
- [ ] Getting key players together to talk through a simulated disaster
- [ ] Sending a fake phishing email to everyone
- [ ] Switching to a redundant router

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Getting key players together to talk through a simulated disaster</p>
<p>Many of the logistics of a disaster response can be determined through analysis and discussion, without actually running a full test.</p>
</details>

---

### 18. What does "fail over" require?
- [ ] A single router and firewall
- [ ] A redundant infrastructure (multiple routers, firewalls, switches) so you can switch to an operational unit if one stops working
- [ ] Shutting down all systems during a failure
- [ ] A cold site

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A redundant infrastructure (multiple routers, firewalls, switches) so you can switch to an operational unit if one stops working</p>
<p>Failure is often inevitable, but with redundancy you may be able to keep running.</p>
</details>

---

### 19. Sending a fake phishing email to everyone in the company to see who bites is an example of what?
- [ ] A tabletop exercise
- [ ] A simulation
- [ ] Parallel processing
- [ ] Fail over

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A simulation</p>
<p>A phishing simulation tests both internal security (did the email get past our filters?) and the users themselves.</p>
</details>

---

### 20. Besides improved performance, what resiliency benefit does parallel processing provide?
- [ ] If one core or CPU fails, processing can be diverted to another
- [ ] It removes the need for backups
- [ ] It encrypts all data automatically
- [ ] It reduces power consumption to zero

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> If one core or CPU fails, processing can be diverted to another</p>
<p>Parallel processing splits a process across multiple CPUs (one computer with multiple cores, or multiple computers) to complete transactions more efficiently.</p>
</details>

---

### 21. What is the trade-off between onsite and offsite backups?
- [ ] Onsite backups need an internet link; offsite backups don't
- [ ] Onsite backups need no internet link and are generally less expensive; offsite backups transfer data over the internet but are available after a disaster
- [ ] Offsite backups are always cheaper
- [ ] There's no trade-off, so organizations only use one

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Onsite backups need no internet link and are generally less expensive; offsite backups transfer data over the internet but are available after a disaster</p>
<p>Organizations often use both, giving them more copies of data and better disaster planning.</p>
</details>

---

### 22. Why should backup media be encrypted?
- [ ] It makes backups faster
- [ ] Backup media holds a history of all the data, so it needs to be protected against attackers, especially for cloud backups
- [ ] Encryption is required for snapshots to work
- [ ] It reduces the size of backups

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Backup media holds a history of all the data, so it needs to be protected against attackers, especially for cloud backups</p>
<p>Encryption is especially useful for cloud backups and storage.</p>
</details>

---

### 23. What is a snapshot?
- [ ] A photo of the server room
- [ ] An instant backup of an entire system, including its current configs and data, popular on VMs and cloud infrastructure
- [ ] A log of user logins
- [ ] A copy of only the changed files

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An instant backup of an entire system, including its current configs and data, popular on VMs and cloud infrastructure</p>
<p>A common approach is to take another snapshot every 24 hours.</p>
</details>

---

### 24. Why isn't performing a backup enough on its own?
- [ ] Backups expire after one day
- [ ] You also need to verify you can restore from it, through disaster recovery testing, confirming the restoration, and periodic audits
- [ ] Backups can't be encrypted
- [ ] Backups always fail

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> You also need to verify you can restore from it, through disaster recovery testing, confirming the restoration, and periodic audits</p>
<p>Simulate a disaster, restore from backup, and test the restored app and data.</p>
</details>

---

### 25. What is replication?
- [ ] A backup done once a month
- [ ] An ongoing, almost real-time backup stored in multiple locations, so even files you just changed have a copy
- [ ] A snapshot of a VM
- [ ] Deleting old backups

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An ongoing, almost real-time backup stored in multiple locations, so even files you just changed have a copy</p>
<p>Replicated data can be stored locally for all users and is recoverable.</p>
</details>

---

### 26. How does journaling prevent data corruption if power goes out while writing to storage?
- [ ] Data is written directly to the database with no intermediate step
- [ ] Data is first written to a journal and then to storage, so if power goes out mid-write, the database can use the journal to redo the actions
- [ ] The journal is deleted before writing begins
- [ ] It keeps a paper copy of all transactions

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data is first written to a journal and then to storage, so if power goes out mid-write, the database can use the journal to redo the actions</p>
<p>If power fails while writing the journal, only the journal is lost and the database isn't corrupted. After data is written to storage, the journal is cleared and the process starts again.</p>
</details>

---

### 27. A UPS protects against blackouts, brownouts, and surges. What is a brownout?
- [ ] Excessive voltage
- [ ] A drop in voltage
- [ ] A complete loss of power
- [ ] A generator failure

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A drop in voltage</p>
<p>A blackout is a complete power loss, a brownout is a drop in voltage, and a surge is excessive voltage. A UPS provides short-term backup power for all of these.</p>
</details>

---

### 28. Which type of UPS turns on only if the power cuts out?
- [ ] Line-interactive UPS
- [ ] Offline/standby UPS
- [ ] On-line UPS
- [ ] Generator

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Offline/standby UPS</p>
<p>A line-interactive UPS increases voltage when it sees a drop on the power line. UPS features include auto shutdown, battery capacity, outlets, and phone line suppression.</p>
</details>

---

### 29. Why is a UPS often used together with a generator?
- [ ] A generator takes a few minutes to get up to speed, so the UPS provides power while it starts
- [ ] Generators can't power an entire building
- [ ] A UPS provides long-term power while the generator handles short-term power
- [ ] Generators don't need fuel

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A generator takes a few minutes to get up to speed, so the UPS provides power while it starts</p>
<p>Generators provide long-term backup power (with fuel) for an entire building or a section of outlets, while a UPS covers the short-term gap.</p>
</details>
