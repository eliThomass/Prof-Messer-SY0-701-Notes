# Quiz 4.7 — Scripting and Automation
*Professor Messer SY0-701 · Section 4.7*

---

### 1. Which is a core reason to automate a security task?
- [ ] It costs nothing to create or implement
- [ ] It never needs updating once it's written
- [ ] It runs without you and without human error
- [ ] It removes every single point of failure

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It runs without you and without human error</p>
<p>Automation runs as fast as the computer it's on and can monitor and resolve problems before they happen, even while you sleep.</p>
</details>

---

### 2. A check finds a server is missing an important security patch. How would automation enforce the baseline?
- [ ] Email the server's owner a reminder
- [ ] Install the patch automatically
- [ ] Add the server to a yearly audit list
- [ ] Remove the server from the baseline

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Install the patch automatically</p>
<p>Enforcing baselines means the missing patch gets installed as soon as it's identified, with no one needing to type anything.</p>
</details>

---

### 3. A team uses a script to build a default router configuration and add firewall rules to each new security appliance. Which benefit is this?
- [ ] Continuous integration and testing
- [ ] User and resource provisioning
- [ ] Workforce multiplier
- [ ] Standard infrastructure configurations

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Standard infrastructure configurations</p>
<p>Scripts can apply IP configs, security rules, and standard config options the same way every time.</p>
</details>

---

### 4. A company orchestrates its cloud resources with automation so security controls grow along with the infrastructure. Which benefit is this?
- [ ] Secure scaling
- [ ] Guard rails
- [ ] Employee retention
- [ ] Technical debt

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Secure scaling</p>
<p>Orchestrating cloud resources with automation ensures proper security scales too.</p>
</details>

---

### 5. Automating the boring work eases the team's workload and leaves them with more rewarding tasks. Which benefit is this?
- [ ] Reaction time
- [ ] Employee retention
- [ ] Secure scaling
- [ ] Escalation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Employee retention</p>
<p>Taking mundane tasks off people's plates makes their work more rewarding, so they're more likely to stay.</p>
</details>

---

### 6. A security event happens and a script addresses it immediately, without waiting for a person. Which benefit is this?
- [ ] Workforce multiplier
- [ ] Ongoing supportability
- [ ] Reaction time
- [ ] Standard infrastructure configurations

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Reaction time</p>
<p>A computer is much faster than we are, so events can be addressed right away.</p>
</details>

---

### 7. Automation takes over repetitive tasks, freeing skilled staff to work somewhere else. Which benefit is this?
- [ ] Reaction time
- [ ] Secure scaling
- [ ] Single point of failure
- [ ] Workforce multiplier

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Workforce multiplier</p>
<p>The same number of people can get more done, because the routine work runs itself.</p>
</details>

---

### 8. When a new employee starts, a script gives them file access, resource access, and the right privileges. Which automation use case is this?
- [ ] User and resource provisioning
- [ ] Ticket creation
- [ ] Escalation
- [ ] Continuous integration and testing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> User and resource provisioning</p>
<p>Provisioning can be automatic for file and resource access, along with privileges.</p>
</details>

---

### 9. What are guard rails in automation?
- [ ] Manual reviews that approve each change before it's deployed
- [ ] Firewall rules that block traffic between network segments
- [ ] Automated validations that limit the behaviors and responses people input
- [ ] Written policies that tell staff which values they're allowed to enter

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Automated validations that limit the behaviors and responses people input</p>
<p>Guard rails reduce errors and constantly check for proper implementation.</p>
</details>

---

### 10. What does automating security groups provide?
- [ ] A yearly manual review of group membership
- [ ] Constant audits without human intervention
- [ ] Permanent group access for every user
- [ ] A separate login for each security group

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Constant audits without human intervention</p>
<p>Automation can assign or remove group access and keep checking it.</p>
</details>

---

### 11. Which is an example of automated ticket creation?
- [ ] A technician types up each reported issue
- [ ] A user phones the help desk with a problem
- [ ] A manager assigns tickets at the end of the day
- [ ] A script turns email submissions into tickets

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A script turns email submissions into tickets</p>
<p>Automation can also identify issues on its own and open tickets for them.</p>
</details>

---

### 12. In automated escalation, when does a human get involved?
- [ ] When the automated fix doesn't resolve the issue
- [ ] Before automation attempts any fix
- [ ] Every time an alert is generated
- [ ] Only during scheduled maintenance windows

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> When the automated fix doesn't resolve the issue</p>
<p>Automation tries to correct the issue first, then contacts the on-call tech if it can't.</p>
</details>

---

### 13. Why automate enabling and disabling services?
- [ ] It keeps every service running at all times
- [ ] It removes the need to monitor services
- [ ] It avoids the "set and forget" habit humans have
- [ ] It lets each user choose which services run

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It avoids the "set and forget" habit humans have</p>
<p>A person might turn a service on and forget about it. A script enables and disables services reliably.</p>
</details>

---

### 14. Why are integrations and APIs useful for automation?
- [ ] They keep scripts from needing any maintenance
- [ ] They let scripts interact with third-party devices and services
- [ ] They limit scripts to a single vendor's products
- [ ] They stop scripts from reaching cloud services

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They let scripts interact with third-party devices and services</p>
<p>Examples include cloud services, firewalls, and operating systems.</p>
</details>

---

### 15. An automation has many moving parts that all have to work together. Which scripting consideration is this?
- [ ] Complexity
- [ ] Cost
- [ ] Technical debt
- [ ] Reaction time

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Complexity</p>
<p>The more pieces that depend on each other, the harder the automation is to get right.</p>
</details>

---

### 16. Which statement about the cost of automation is true?
- [ ] Scripts are free because no one has to type
- [ ] Cost only applies to cloud-based automation
- [ ] Automation has no cost after the first year
- [ ] It takes money to create and implement a script

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It takes money to create and implement a script</p>
<p>Automation saves time, but that doesn't make it free to build.</p>
</details>

---

### 17. All of a company's account creation runs through one script. If the script stops working, no accounts get created. Which risk is this?
- [ ] Technical debt
- [ ] Single point of failure
- [ ] Ongoing supportability
- [ ] Guard rails

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Single point of failure</p>
<p>When a process depends on one script, the process stops if the script does.</p>
</details>

---

### 18. A team keeps patching over a problem, pushing the real fix down the road where it will cost more. What is this called?
- [ ] Complexity
- [ ] Ongoing supportability
- [ ] Technical debt
- [ ] Single point of failure

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Technical debt</p>
<p>Quick patches can delay the issue rather than solve it, and it'll be more expensive to fix later.</p>
</details>

---

### 19. A script works great today, but it may not keep working as things change. Which consideration is this?
- [ ] Ongoing supportability
- [ ] Technical debt
- [ ] Cost
- [ ] Complexity

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Ongoing supportability</p>
<p>A script isn't finished once it's deployed. It needs support to keep working over time.</p>
</details>
