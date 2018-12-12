# Security in OpenAPI
Philippe Leothaud

## Security is a layered approach
- System
- Network
- Application

## Infrastructure
Http, rest & json

Targets

- Own product Internal
- Own product in cloud
- External

## Security goals
- Integrity
- Confidentiality (not intercepted)
- Availability (DOS attacks)
- Authentication
- Authorization
- Audit
- Non-repudiation (proof)

## Integrity/Confidentiality
- Transport (TLS)
- Message (encryption/signature)

### Transport is good, but not enough.

- SSL TLS problems (1.2 or 1.3 to be used)
- Logs contain urls with (sensitive) data
- P2P is not enough: other API calls (Apple Pay/banking/…)

### Message level security
Two standards:

- JOSE/JWT (-> look up JOSE)
- HTTP

## Availability
- Network level
- Application level (throttling)

## Authentication
- OAuth
- OpenID connect

## Authorization
- OAuth

## Challenges API infrastructure
- System security: don’t assume clients are secure
- Network security: more and more endpoints
- Application security: Agility -> makes it harder to be secure: tools are needed (sec devops)

## OpenApi 3.0.2
- Security schemes (global securityDefinitions of the component)
- Security requirements (security field: array with logical OR)

Current schemes:

- http
- apiKey
- oauth2
- openidconnect

⇒ `security` -> OR

## Data validation

Json schema:

- String
 - Format
 - Pattern
 - Maxlenght
 - Minlength
- Numbers
 - format 
 - multipleOf
 - Minimum
 - Maximum
 - Exclusive minimum
 - Exclusive max
- Array
 - Items
 - Maxitems
 - Minitems

## What is missing?
- Mutual tls
- Extensions to oath
 - Pkce support
 - Token binding
- Confidentiality and integrity -> message-level crypto
 - Extend with cryptographic definitions
