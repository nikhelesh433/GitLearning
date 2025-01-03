# Authenticaton Mechanisims
1. Password-Based Authentication
2. Multi-Factor Authentication (MFA) or (2FA)
3. Biometric Authentication
4. Token-Based Authentication
5. Certificate-Based Authentication
6. Single Sign-On (SSO)
7. OAuth and OpenID Connect
8. Behavioral Authentication
9. Risk-Based Authentication
10. Hardware Security Modules (HSM)


### 1. Password-Based Authentication
Requires users to provide a user id and password.

### 2. Multi-Factor Authentication (MFA) or (2FA)
It combines two or more authentication factors for example
Something you know: Password or PIN.
Something you have: Mobile device, security token.
Something you are: Biometric data (fingerprint, facial recognition).

### 3. Biometric Authentication
Uses physical or behavioral characteristics such as:
Fingerprints
Face recognition
Iris or retina scans

### 4. Token-Based Authentication
Uses a token (physical or digital) to verify identity. Examples:
Hardware tokens (key fobs)
Software tokens (Using a YubiKey or receiving OTP from apps like Google Authenticator)

### 5. Certificate-Based Authentication
Uses digital certificates issued by a trusted Certificate Authority (CA). The certificates are encrypted files a public and a private key. 

### 6. Single Sign-On (SSO)
Allows users to log in once and access multiple systems.
It works as we authenticate ourself with an account and from then on we can use it. For example we try to log in to our spotify account using google(identity proivider), Google checks if the user is authenticated otherwise it asks to authenticate self by provding credentials. Once google validates the credentials, it wll send a token back to spotify and spotify redirects to the pre-defined page(home).
I companies we use Single sign-ons as they authenticate users based on their employe credentials.

### 7. OAuth and OpenID Connect
Protocols used for delegated authentication and authorization.

### 8. Behavioral Authentication
Monitors user behavior (e.g., typing patterns, mouse movements).

### 9. Risk-Based Authentication
Adjusts the authentication process based on the risk level (e.g., login location, time).

### 10. Hardware Security Modules (HSM)
Dedicated hardware devices for secure key storage and authentication.







AuthN (Authentication) and AuthZ (Authorization) are two fundamental concepts in cybersecurity, and while they are closely related, they serve distinct purposes:

Authentication (AuthN)
Definition: Authentication is the process of verifying the identity of a user, system, or entity. It ensures that the entity requesting access is who they claim to be.

Examples of Authentication:

Logging in with a username and password.
Scanning a fingerprint or using facial recognition.
Entering a one-time password (OTP) sent via email or SMS.
Using a hardware token or smart card.
Analogy: Think of it as showing your ID card at a security checkpoint to prove your identity.

Authorization (AuthZ)
Definition: Authorization is the process of determining what resources a verified user, system, or entity is permitted to access. It happens after authentication.

Examples of Authorization:

A verified user can read files but cannot edit or delete them.
A manager has access to sensitive financial data, while regular employees do not.
A guest user can only view public information on a website.
Analogy: Once your ID card is accepted, the guard checks a list to see if you're allowed to enter certain areas.

Key Differences Between AuthN and AuthZ
Aspect	Authentication (AuthN)	Authorization (AuthZ)
Purpose	Verify identity	Define access rights
When it occurs	Before authorization	After authentication
Focus	"Who are you?"	"What are you allowed to do?"
Techniques/Tools	Passwords, biometrics, tokens, MFA	Access control lists (ACLs), roles, policies
Output	Validated identity	Permissions to access resources
Real-Life Example:
AuthN: You log into your email account by entering your credentials.
→ The system confirms it’s you.
AuthZ: After logging in, you can send and receive emails, but you can't access the admin panel unless you are an administrator.
→ The system decides what actions you can perform.
Would you like examples of how AuthN and AuthZ are implemented in systems like APIs or cloud environments?