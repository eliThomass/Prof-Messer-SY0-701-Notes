# Quiz 1.3 — Change Management
*Professor Messer SY0-701 · Section 1.3*

---

### 1. What is the purpose of a backout plan?
- [ ] To document who approved the change
- [ ] To revert back to the original version before the change took place
- [ ] To schedule the next maintenance window
- [ ] To track version history of a configuration file

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To revert back to the original version before the change took place</p>
<p>The backout plan reverts back to the original version before the change took place. This is usually easy, but some changes are very difficult, so good backups are essential.</p>
</details>

---

### 2. Why is a sandbox testing environment used before making a change to production?
- [ ] To permanently host the new configuration
- [ ] To test the change and confirm the backout plan works
- [ ] To notify stakeholders of the change
- [ ] To bypass the change approval process

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To test the change and confirm the backout plan works</p>
<p>A sandbox environment is used before making a change to production, to confirm the backout plan will work if needed.</p>
</details>

---

### 3. Which application control approach is described as "nothing runs unless it's approved," making it very restrictive?
- [ ] Deny list
- [ ] Allow list
- [ ] Version control
- [ ] Change control board

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Allow list</p>
<p>An allow list means nothing runs unless it's approved, which is very restrictive. A deny list is more flexible: nothing on the bad list can be executed, but everything else is permitted.</p>
</details>

---

### 4. In change management, who typically owns the process versus who implements the actual change?
- [ ] IT owns the process; a department implements the change
- [ ] A department owns the process; IT usually implements the actual change
- [ ] Stakeholders own and implement the change together
- [ ] The change control board implements the change directly

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A department owns the process; IT usually implements the actual change</p>
<p>An individual/owner manages the change management process and ensures it's followed, but usually the actual change is implemented by IT.</p>
</details>

---

### 5. What is Impact Analysis primarily concerned with determining?
- [ ] The exact time the change will occur
- [ ] A risk value for the change, including the risk of NOT making it
- [ ] Which stakeholders approved the request form
- [ ] The version history of the affected system

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A risk value for the change, including the risk of NOT making it</p>
<p>Impact analysis determines a risk value (minor or far-reaching) and also considers the risk of not making the change, such as security vulnerabilities or unexpected downtime.</p>
</details>

---

### 6. Why are maintenance windows often scheduled overnight rather than during the workday?
- [ ] Overnight changes never require a backout plan
- [ ] To minimize impact on users and production systems during business hours
- [ ] IT staff are only available overnight
- [ ] Change control boards only meet overnight

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To minimize impact on users and production systems during business hours</p>
<p>Scheduling a change is often the most difficult part of the process; making changes during the workday is usually not ideal, so overnight windows are often a better choice.</p>
</details>

---

### 7. A change that requires updating the firewall code before modifying another connected system is an example of what?
- [ ] A dependency
- [ ] A backout plan
- [ ] Version control
- [ ] An allow list

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A dependency</p>
<p>Dependencies mean that to complete one change, another must be completed first — modifying one component may require changing or restarting other components, sometimes across systems.</p>
</details>

---

### 8. Which of the following is typically required as part of the change management documentation process?
- [ ] Updating diagrams and address information
- [ ] Deleting old configuration backups
- [ ] Disabling the change control board
- [ ] Skipping end-user acceptance

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Updating diagrams and address information</p>
<p>Documentation is often required with the change management process, including updating diagrams, address updates, and updating policies/procedures.</p>
</details>

---

### 9. What is version control used for in technical change management?
- [ ] Approving change requests from stakeholders
- [ ] Tracking changes to a file or configuration data over time, such as router configs or OS patches
- [ ] Scheduling the maintenance window
- [ ] Testing a change in a sandbox environment

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Tracking changes to a file or configuration data over time, such as router configs or OS patches</p>
<p>Version control tracks changes to files or configuration data over time (e.g. router configs, Windows OS patches, application registry entries), and may require additional management software.</p>
</details>

---

### 10. Why must stakeholders have input on the change management process?
- [ ] They are legally required to approve every IT ticket
- [ ] A change to one system, like shipping label software, can affect many other groups (e.g. accounting, receiving, delivery timeframes)
- [ ] They perform the technical implementation of the change
- [ ] They write the backout plan

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A change to one system, like shipping label software, can affect many other groups (e.g. accounting, receiving, delivery timeframes)</p>
<p>Stakeholders want input because a change could affect one individual or the whole company — e.g. updating shipping label software impacts shipping/receiving, accounting reports, delivery timeframes, and revenue recognition.</p>
</details>

---

### 11. Why is it important to have a well-documented change control process regarding "restricted activities"?
- [ ] Because approval for a change isn't permission to make any change, and scope may need to expand during the window
- [ ] Because it eliminates the need for a maintenance window
- [ ] Because it replaces the need for stakeholder approval
- [ ] Because it allows any technician to skip the approval process

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Because approval for a change isn't permission to make any change, and scope may need to expand during the window</p>
<p>A change approval isn't blanket permission to make any change — scope may need to be expanded during the change window, which is why a well-documented change control process matters.</p>
</details>

---

### 12. What approach does the course recommend for dealing with legacy applications during change management?
- [ ] Avoid changing them entirely, forever
- [ ] Replace them immediately regardless of cost
- [ ] Become the expert and learn the application's quirks
- [ ] Ignore them since they are unsupported

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Become the expert and learn the application's quirks</p>
<p>Legacy applications often create fear of the unknown since no one understands them anymore — the recommended approach is to become the expert and conquer the quirks.</p>
</details>
