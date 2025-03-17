### Describe directory services in Azure, including Microsoft Entra ID and Microsoft Entra Domain Services

**Entra ID** identityand access management service, authentication for accessing resources,uses OAuth or SAML authentication.  

**Entra ID DS** is a domain service that allows the use of older authentication methods (Kerberos/NTLM) for legacy applications.

### Describe authentication methods in Azure, including single sign-on (SSO), multifactor authentication, and passwordless
- SSO: Single login for multiple services.
- MFA: Adds extra verification like codes or biometrics.
- Passwordless: Use PIN or fingerprint after device registration. Microsoft Authenticator supports both MFA and passwordless.

### Describe external identities and guest access in Azure
Consumers can use non-MS credentials to access resources. Authorization is managed via Azure Entra ID.

### Describe Microsoft Entra Conditional Access
Enforces organizational policies, access is granted or revoked based on signals like identity, device, or location. You can also require MFA instead of blocking the user.


### Describe Azure role-based access control (RBAC)
Create roles with a set of permissions and assign them to a scope, such as a subscription etc, instead of assigning permissions manually.

### Describe the concept of Zero Trust
Authenticate every time. Give minimal permissions required. Deny by default.  

### Describe the purpose of the defense in depth model
A layered approach to security. Starting from the outermost layer:
- Physical: 
- Identity & Access: 
- Perimeter: DDoS attacks
- Network: inbound and outbound internet access should be limited
- Compute: VM's should be protected (e.g. require SSH)
- Application: remove security vulnerabilities within your application 
- Data: protect the database or disk storage

### Describe the purpose of Microsoft Defender for Cloud
Built-in for cloud services. Three components:
1. Continuously Assess: automatically run vulnerability scans
2. Secure: set security policies and follow compliance best practices through Azure Security Benchmark
3. Alerts: get notified, suggested remediation steps, option to trigger logic in response to an alert.
