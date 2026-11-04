# Quiz 4.6 — Identity and Access Management
*Professor Messer SY0-701 · Section 4.6*

---

### 1. What is the overall goal of Identity and Access Management (IAM)?
- [ ] Give every user the same permissions across all systems
- [ ] Encrypt all data stored on the network
- [ ] Give the right permissions to the right people at the right time
- [ ] Replace passwords with biometrics

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Give the right permissions to the right people at the right time</p>
<p>IAM covers identity lifecycle management, access control, authentication and authorization, and identity governance.</p>
</details>

---

### 2. Which part of IAM tracks an entity's resource access?
- [ ] Identity governance
- [ ] Identity proofing
- [ ] Provisioning
- [ ] Federation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Identity governance</p>
<p>Access control makes sure an entity only gets what it needs, and authentication makes entities prove they are who they claim.</p>
</details>

---

### 3. Which event would normally trigger provisioning or de-provisioning of a user account?
- [ ] A password manager update
- [ ] A scheduled vulnerability scan
- [ ] A hire, transfer, promotion, or job separation
- [ ] A firewall rule change

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A hire, transfer, promotion, or job separation</p>
<p>Provisioning and de-provisioning are the account creation and removal process, and an initial checkpoint for limiting access.</p>
</details>

---

### 4. How much access should an entity get under permission assignments?
- [ ] Full access until a problem is reported
- [ ] The same access as its manager
- [ ] Privileged OS access on its user account
- [ ] Just enough permissions to do its job

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Just enough permissions to do its job</p>
<p>Group assignments are common, storage and files can be private to a user, and user accounts get no privileged OS access.</p>
</details>

---

### 5. In identity proofing, which step is "who the system thinks you are"?
- [ ] Resolution
- [ ] Validation
- [ ] Verification
- [ ] Attestation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Resolution</p>
<p>Validation gathers information from the user, like a password or security questions. Verification (or attestation) requires extra proof.</p>
</details>

---

### 6. A new employee must show a passport at an in-person meeting to prove their identity. Which identity proofing step is this?
- [ ] Resolution
- [ ] Validation
- [ ] Verification
- [ ] Provisioning

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Verification</p>
<p>Verification, also called attestation, uses extra details to prove identity.</p>
</details>

---

### 7. What does single sign-on (SSO) provide?
- [ ] A separate password for each application you use
- [ ] Credentials entered once, with no additional authentication
- [ ] Permanent access that never expires or needs renewal
- [ ] Automatic admin rights on every connected system

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Credentials entered once, with no additional authentication</p>
<p>Without SSO, you'd need a username and password every time.</p>
</details>

---

### 8. Which is true about SSO?
- [ ] It works with any authentication process, with no changes needed
- [ ] It removes the need for an authentication server on the network
- [ ] It's only available on mobile devices that support biometrics
- [ ] It's usually time-limited, and the underlying authentication must support it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's usually time-limited, and the underlying authentication must support it</p>
<p>For example, an SSO session might have a 24-hour limit.</p>
</details>

---

### 9. What is LDAP used for?
- [ ] Reading and writing directories over an IP network
- [ ] Signing outgoing email
- [ ] Encrypting wireless traffic
- [ ] Scanning networks for open ports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Reading and writing directories over an IP network</p>
<p>LDAP stands for Lightweight Directory Access Protocol.</p>
</details>

---

### 10. How is an X.500 distinguished name ordered?
- [ ] Alphabetically
- [ ] Most general attribute first
- [ ] Most specific attribute first
- [ ] In random order

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Most specific attribute first</p>
<p>X.500 distinguished names list the most specific attribute at the start.</p>
</details>

---

### 11. In the X.500 Directory Information Tree, which are examples of container objects?
- [ ] Printers, laptops, and mobile phones
- [ ] Country, organization, and organizational units
- [ ] Usernames, passwords, and security questions
- [ ] Signatures, public keys, and certificates

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Country, organization, and organizational units</p>
<p>The tree's hierarchical structure is built from container objects and leaf objects.</p>
</details>

---

### 12. What does SAML allow?
- [ ] Authenticating through a third party to gain access
- [ ] Filtering websites by reputation
- [ ] Checking devices for the latest patches
- [ ] Storing passwords in an encrypted vault

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Authenticating through a third party to gain access</p>
<p>Security Assertion Markup Language is an open standard for authentication and authorization.</p>
</details>

---

### 13. What is a known limitation of SAML?
- [ ] It's a proprietary standard
- [ ] It doesn't support authentication
- [ ] It requires a hardware token
- [ ] It wasn't originally designed for mobile apps

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It wasn't originally designed for mobile apps</p>
<p>SAML is a good fit for traditional third-party authentication, but mobile apps weren't part of its original design.</p>
</details>

---

### 14. You click "Allow" so an app can see and edit your Google Drive files. Which technology is this?
- [ ] LDAP
- [ ] X.500
- [ ] OAuth
- [ ] DMARC

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> OAuth</p>
<p>OAuth is an authorization framework, created by Twitter, Google, and others, that determines which resources a user can access.</p>
</details>

---

### 15. OAuth is not an authentication protocol. What is it used with to handle authentication?
- [ ] OpenID
- [ ] SNMP
- [ ] Tripwire
- [ ] SPF

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> OpenID</p>
<p>OAuth handles what you can access (authorization), and OpenID handles proving who you are (authentication).</p>
</details>

---

### 16. What does federation require before third parties can share authentication?
- [ ] A shared physical network
- [ ] A trust relationship between the parties
- [ ] A local authentication database at each site
- [ ] Identical password policies

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A trust relationship between the parties</p>
<p>Federation provides network access to others, including SSO, without a local authentication database. "Log in with Google" is a common example.</p>
</details>

---

### 17. A VPN concentrator authenticates users against the organization's LDAP server, while a new app needs OAuth. What does this show about authentication interoperability?
- [ ] LDAP and OAuth can't exist in the same organization
- [ ] Every app must use the same authentication method
- [ ] OAuth has replaced LDAP
- [ ] It depends on the environment and what's at hand

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It depends on the environment and what's at hand</p>
<p>There are many ways to communicate with an authentication server. For the new app, the organization would need to allow authentication API access for OAuth.</p>
</details>

---

### 18. What is authorization?
- [ ] The process of ensuring only authorized rights are exercised
- [ ] The process of proving who you are
- [ ] The process of creating a user account
- [ ] The process of logging user activity

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The process of ensuring only authorized rights are exercised</p>
<p>Users receive these rights based on access control models.</p>
</details>

---

### 19. Under the principle of least privilege, which is the right setup for a regular user account?
- [ ] Admin rights, in case they're needed
- [ ] Rights set to the bare minimum necessary
- [ ] The same rights as the IT team
- [ ] No rights at all

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Rights set to the bare minimum necessary</p>
<p>All user accounts must be limited, and users shouldn't run with admin privileges.</p>
</details>

---

### 20. Every object has a label like "secret" or "top secret," and the OS enforces access by clearance level. Users can't change this. Which access control model is this?
- [ ] Discretionary access control
- [ ] Role-based access control
- [ ] Mandatory access control
- [ ] Rule-based access control

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Mandatory access control</p>
<p>Labeling follows predefined rules that set who has access and who can write.</p>
</details>

---

### 21. You create a spreadsheet and decide who can open it. Which access control model is this?
- [ ] Mandatory access control
- [ ] Attribute-based access control
- [ ] Rule-based access control
- [ ] Discretionary access control

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Discretionary access control</p>
<p>The owner controls access and can modify it at any time. DAC is used in most operating systems and is very flexible, but its security is very weak.</p>
</details>

---

### 22. A new team lead is added to the "Team Leads" group and automatically gets that group's access. Which access control model is this?
- [ ] Role-based access control
- [ ] Discretionary access control
- [ ] Mandatory access control
- [ ] Time-of-day restrictions

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Role-based access control</p>
<p>Admins provide access based on the user's role, and rights are gained implicitly from the group. Windows uses Groups to provide RBAC.</p>
</details>

---

### 23. "Lab network access is only available between 9AM and 5PM" and "Only Chrome browsers may complete a web form" are examples of which model?
- [ ] Role-based access control
- [ ] Rule-based access control
- [ ] Discretionary access control
- [ ] Mandatory access control

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Rule-based access control</p>
<p>System admins configure system-enforced rules. Each rule is associated with a specific object, and the system checks the ACLs for that object.</p>
</details>

---

### 24. A system weighs IP address, time of day, desired action, and relationship to the data before granting access. Which model is this?
- [ ] Rule-based access control
- [ ] Discretionary access control
- [ ] Mandatory access control
- [ ] Attribute-based access control

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Attribute-based access control</p>
<p>ABAC is a next-generation authorization model that's aware of context and evaluates multiple parameters together.</p>
</details>

---

### 25. Why can time-of-day restrictions be difficult to implement?
- [ ] Few security devices support them
- [ ] They require biometric authentication
- [ ] A worldwide organization works across many time zones
- [ ] They only work with mandatory access control

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A worldwide organization works across many time zones</p>
<p>Almost all security devices include a time-of-day option for restricting access during certain times or days of the week.</p>
</details>

---

### 26. Which login combines two different authentication factors?
- [ ] A password and a PIN
- [ ] A fingerprint and an iris scan
- [ ] A PIN and a pattern
- [ ] A password and a USB security key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A password and a USB security key</p>
<p>A password is something you know and a USB key is something you have. In the other options, both items come from the same factor.</p>
</details>

---

### 27. Which is an example of "something you have"?
- [ ] A smart card
- [ ] A PIN
- [ ] A voice print
- [ ] An IP address

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A smart card</p>
<p>Others include USB security keys, hardware and software tokens, and your phone receiving an SMS.</p>
</details>

---

### 28. What does biometric authentication usually store?
- [ ] A photo of your fingerprint
- [ ] A mathematical representation of your biometric
- [ ] An encrypted copy of your password
- [ ] A recording of your voice

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A mathematical representation of your biometric</p>
<p>Biometrics are difficult to change, unlike a password, and aren't foolproof, so they're used with other factors.</p>
</details>

---

### 29. A transaction only completes if the user is in a particular geography. Which factor is this?
- [ ] Something you know
- [ ] Something you have
- [ ] Something you are
- [ ] Somewhere you are

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Somewhere you are</p>
<p>Location can come from an IP address or mobile device location services.</p>
</details>

---

### 30. What does increasing password entropy do?
- [ ] Makes the password more unpredictable, so it better resists brute force
- [ ] Makes the password easier to remember between expiration dates
- [ ] Shortens the time until the password expires and must be changed
- [ ] Stores the password in a shared and encrypted password database

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Makes the password more unpredictable, so it better resists brute force</p>
<p>Stronger passwords are commonly at least 8 characters.</p>
</details>

---

### 31. What is the difference between password age and password expiration?
- [ ] Age is the time until it expires; expiration is the time since it was created
- [ ] Age is how long since the password was modified; expiration means it only works for a certain amount of time
- [ ] Age is set by the user; expiration is set by the vendor
- [ ] They mean the same thing

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Age is how long since the password was modified; expiration means it only works for a certain amount of time</p>
<p>The system admin determines the time, and the system remembers password history.</p>
</details>

---

### 32. Why use a password manager?
- [ ] So you can reuse one strong password everywhere
- [ ] So your passwords are stored in plain text for quick access
- [ ] So you can use a different password for every account, stored in one encrypted database
- [ ] So that you never need to log in with multifactor authentication

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> So you can use a different password for every account, stored in one encrypted database</p>
<p>Password managers are built into many operating systems and some browsers, can include multifactor tokens for login, and come in enterprise versions.</p>
</details>

---

### 33. Which is an example of passwordless authentication?
- [ ] A long, complex password
- [ ] A PIN sent to your email
- [ ] Single sign-on with a shared password
- [ ] Facial recognition or a security key

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Facial recognition or a security key</p>
<p>Many breaches come from poor password control, and passwordless authentication solves many of those issues. It may be used alongside other methods rather than as the primary one.</p>
</details>

---

### 34. How do just-in-time permissions reduce risk?
- [ ] Admin access is temporary, so a breached account has no elevated rights
- [ ] Every IT user keeps a permanent admin account that's closely monitored
- [ ] Users log in to every system with one shared admin password
- [ ] Admin rights are granted automatically each time a user logs in

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Admin access is temporary, so a breached account has no elevated rights</p>
<p>This follows the principle of least privilege and narrows the scope of a breach.</p>
</details>

---

### 35. With just-in-time permissions, what happens when a user needs elevated access?
- [ ] They ask a coworker in IT for the shared admin password
- [ ] They request it from a password vault, which creates a temporary account
- [ ] Their regular account is permanently promoted to an admin account
- [ ] They turn off the firewall until the elevated task is finished

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They request it from a password vault, which creates a temporary account</p>
<p>The vault is a central clearinghouse that sets different controls for each user. The temporary account has elevated privileges and is deleted after the session.</p>
</details>
