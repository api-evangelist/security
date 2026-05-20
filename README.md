# Security (security)
An index and topic collection covering API security, identity, access management, secrets management, encryption, and threat protection. API security spans the full lifecycle of an API, from designing strong authentication and authorization, to managing keys, secrets, and certificates, to protecting runtime traffic with WAFs, rate limiting, and bot mitigation, to scanning code and dependencies for vulnerabilities. This collection brings together identity providers like Okta, Auth0, and Keycloak; secrets and key management platforms like HashiCorp Vault and AWS KMS; cloud security and WAF vendors like Cloudflare, Akamai, and Palo Alto Networks; and software supply chain security tools like Snyk, Sigstore, and Sonatype.

**URL:** [https://apievangelist.com](https://apievangelist.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - API Security, Identity and Access Management, Authentication, Secrets Management, Threat Protection

## Timestamps

- **Created:** 2026-05-19
- **Modified:** 2026-05-19

## Common Properties

- [Portal](https://apievangelist.com)
- [GitHubOrganization](https://github.com/api-evangelist)
- [JSONSchema - OAuth Client Schema](https://raw.githubusercontent.com/api-evangelist/security/refs/heads/main/json-schema/security-oauth-client-schema.json)
- [JSONSchema - Secret Schema](https://raw.githubusercontent.com/api-evangelist/security/refs/heads/main/json-schema/security-secret-schema.json)
- [JSON-LD](https://raw.githubusercontent.com/api-evangelist/security/refs/heads/main/json-ld/security-context.jsonld)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/security/refs/heads/main/vocabulary/security-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Authentication and Identity | Identity platforms like Okta, Auth0, Keycloak, and Microsoft Entra provide OAuth 2.0, OIDC, SAML, and social login flows so APIs do not have to roll their own authentication. |
| Authorization and Fine-Grained Access | Tools like OpenFGA, Ory, Amazon Verified Permissions, and SailPoint implement role-based, attribute-based, and relationship-based access control at the API and resource level. |
| Secrets and Key Management | Platforms like HashiCorp Vault, AWS KMS, Azure Key Vault, and 1Password centralize the storage, rotation, and auditing of API keys, tokens, database credentials, and encryption keys. |
| API Threat Protection and WAF | Edge security platforms like Cloudflare, Akamai, Amazon WAF, and Fortinet inspect API traffic for OWASP API Top 10 attacks, bot abuse, credential stuffing, and DDoS at the network edge. |
| API Security Posture and Scanning | Specialized API security tools like 42Crunch, Traceable, and Salt scan OpenAPI specifications and live traffic for misconfigurations, broken authentication, and excessive data exposure. |
| Software Supply Chain Security | Tools like Snyk, Sonatype, JFrog Xray, Sigstore, and Trivy scan code, dependencies, containers, and artifacts for vulnerabilities and verify provenance before APIs reach production. |
| Runtime and Workload Security | Runtime security platforms like Falco, Sysdig, Aqua Security, and StackRox monitor containers and Kubernetes workloads that host APIs for suspicious behavior and policy violations. |
| Certificate and TLS Management | Certificate authorities and managers like Let's Encrypt, DigiCert, and AWS Private CA issue, rotate, and revoke TLS certificates that secure API endpoints in transit. |

## Use Cases

| Name | Description |
|------|-------------|
| OAuth 2.0 and OIDC for API Access | Use an identity provider like Okta, Auth0, or Keycloak to issue access tokens and ID tokens that API gateways and services validate on every request. |
| Centralized Secrets for Microservices | Replace hard-coded credentials with short-lived secrets fetched from HashiCorp Vault or AWS Secrets Manager so each service authenticates with its own dynamically issued identity. |
| WAF and Bot Mitigation in Front of APIs | Place a WAF like Cloudflare or Akamai in front of public APIs to block OWASP API Top 10 attacks, credential stuffing, scraping bots, and volumetric DDoS before they reach origin. |
| API Security Testing in CI/CD | Integrate API security scanners like 42Crunch and dependency scanners like Snyk into CI/CD pipelines so vulnerabilities are caught before APIs ship. |
| Privileged Access Management | Use CyberArk, BeyondTrust, or 1Password to broker, monitor, and rotate access to administrative APIs and infrastructure credentials. |
| Zero Trust and Workload Identity | Issue cryptographic workload identities with SPIFFE/SPIRE so services authenticate to APIs using verifiable identities instead of static API keys. |
| Vulnerability and Posture Management | Continuously scan APIs, hosts, containers, and cloud accounts with Qualys, Rapid7, CrowdStrike, or Sysdig to detect exposed endpoints and misconfigurations. |
| Signed Artifacts and Supply Chain Attestation | Use Sigstore, Sonatype, and JFrog Xray to sign, verify, and attest the provenance of API server images and their dependencies. |

## Integrations

| Name | Description |
|------|-------------|
| Okta | Identity platform providing OAuth 2.0, OIDC, SAML, MFA, and lifecycle management for workforce and customer identities accessing APIs. |
| Auth0 | Developer-friendly identity platform (now part of Okta) for adding authentication, social login, and authorization to APIs. |
| HashiCorp Vault | Secrets management platform for storing, rotating, and dynamically issuing API tokens, database credentials, certificates, and encryption keys. |
| Cloudflare | Global edge platform providing WAF, API Shield, bot management, rate limiting, mTLS, and DDoS protection for APIs. |
| Snyk | Developer-first security platform that scans code, dependencies, containers, and IaC for vulnerabilities affecting API services. |
| Keycloak | Open-source identity and access management server implementing OAuth 2.0, OIDC, and SAML for protecting APIs and applications. |
| Sigstore | Open-source project for signing, verifying, and proving the provenance of software artifacts used in API supply chains. |
| 42Crunch | API security platform that audits OpenAPI definitions, scans live APIs, and enforces security policies at the gateway. |

## Artifacts

Machine-readable API specifications organized by format.

### JSON Schema

- [OAuth Client Schema](json-schema/security-oauth-client-schema.json)
- [Secret Schema](json-schema/security-secret-schema.json)

### JSON Structure

- [OAuth Client Structure](json-structure/security-oauth-client-structure.json)
- [Secret Structure](json-structure/security-secret-structure.json)

### JSON-LD

- [Security Context](json-ld/security-context.jsonld)

## Vocabulary

- [Security Vocabulary](vocabulary/security-vocabulary.yaml) - Unified taxonomy mapping resources, actions, workflows, and personas across identity, secrets, and API threat protection.

## Network

This index references the following API security and identity repositories:

- [1Password](https://github.com/api-evangelist/1password)
- [42Crunch](https://github.com/api-evangelist/42crunch)
- [Akamai](https://github.com/api-evangelist/akamai)
- [Amazon Cognito](https://github.com/api-evangelist/amazon-cognito)
- [Amazon GuardDuty](https://github.com/api-evangelist/amazon-guardduty)
- [Amazon IAM](https://github.com/api-evangelist/amazon-iam)
- [Amazon KMS](https://github.com/api-evangelist/amazon-kms)
- [Amazon Secrets Manager](https://github.com/api-evangelist/amazon-secrets-manager)
- [Amazon Security Hub](https://github.com/api-evangelist/amazon-security-hub)
- [Amazon Shield](https://github.com/api-evangelist/amazon-shield)
- [Amazon WAF](https://github.com/api-evangelist/amazon-waf)
- [Aqua Security](https://github.com/api-evangelist/aqua-security)
- [Auth0](https://github.com/api-evangelist/auth0)
- [Authelia](https://github.com/api-evangelist/authelia)
- [BeyondTrust](https://github.com/api-evangelist/beyondtrust)
- [Check Point](https://github.com/api-evangelist/checkpoint)
- [Cilium](https://github.com/api-evangelist/cilium)
- [Cloudflare](https://github.com/api-evangelist/cloudflare)
- [CrowdStrike](https://github.com/api-evangelist/crowdstrike)
- [CyberArk](https://github.com/api-evangelist/cyberark)
- [Digicert](https://github.com/api-evangelist/digicert)
- [Duo Security](https://github.com/api-evangelist/duo-security)
- [F5 Networks](https://github.com/api-evangelist/f5-networks)
- [Falco](https://github.com/api-evangelist/falco)
- [ForgeRock](https://github.com/api-evangelist/forgerock)
- [Fortinet](https://github.com/api-evangelist/fortinet)
- [HashiCorp Vault](https://github.com/api-evangelist/hashicorp-vault)
- [JFrog](https://github.com/api-evangelist/jfrog)
- [JumpCloud](https://github.com/api-evangelist/jumpcloud)
- [Keycloak](https://github.com/api-evangelist/keycloak)
- [Let's Encrypt](https://github.com/api-evangelist/lets-encrypt)
- [Logto](https://github.com/api-evangelist/logto)
- [Microsoft Entra](https://github.com/api-evangelist/microsoft-entra)
- [Okta](https://github.com/api-evangelist/okta)
- [OneLogin](https://github.com/api-evangelist/onelogin)
- [OpenFGA](https://github.com/api-evangelist/openfga)
- [Ory](https://github.com/api-evangelist/ory)
- [Palo Alto Networks](https://github.com/api-evangelist/palo-alto-networks)
- [Ping Identity](https://github.com/api-evangelist/ping-identity)
- [Qualys](https://github.com/api-evangelist/qualys)
- [Rapid7](https://github.com/api-evangelist/rapid7)
- [SailPoint](https://github.com/api-evangelist/sailpoint)
- [Sigstore](https://github.com/api-evangelist/sigstore)
- [Snyk](https://github.com/api-evangelist/snyk)
- [Sonatype](https://github.com/api-evangelist/sonatype)
- [SPIFFE](https://github.com/api-evangelist/spiffe)
- [StackRox](https://github.com/api-evangelist/stackrox)
- [SuperTokens](https://github.com/api-evangelist/supertokens)
- [Symantec](https://github.com/api-evangelist/symantec)
- [Sysdig](https://github.com/api-evangelist/sysdig)
- [Trivy](https://github.com/api-evangelist/trivy)
- [Veracode](https://github.com/api-evangelist/veracode)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
