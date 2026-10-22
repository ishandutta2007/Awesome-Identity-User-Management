# Awesome-Identity-User-Management

## Top Identity & User Management Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Authentication, Authorization & Self-Hosted Identity Infrastructure*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Identity & User Management**. These tools provide the authentication and authorization layer for applications—managing user identities, sessions, single sign-on, and access control—so teams don't have to build and maintain security-critical infrastructure themselves.



**Examples** include Auth0, Okta, Microsoft Entra ID, Ping Identity (ForgeRock), OneLogin, JumpCloud, WorkOS, and Keycloak (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, avoiding per-MAU pricing, and retaining full control over user data—ideal for organizations that need data sovereignty, predictable costs, and auditable identity flows. The open-source landscape is anchored by **Keycloak** (the enterprise standard with the broadest protocol support and 25K+ GitHub stars), **Authentik** (the modern alternative with better UX and flexible flow engine), **Ory** (the headless, composable building blocks for custom auth), and **Zitadel** (the cloud-native multi-tenant IdP), with **Authelia** serving reverse-proxy authentication needs and **Casdoor** offering a Go-based alternative with built-in MCP server support.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global Identity and Access Management (IAM) market is estimated at **$24B–$30B in 2025–2026** and continues to grow at double-digit CAGR driven by Zero Trust initiatives, cloud migration, and AI workload security. The sector is **moderately concentrated at the top with a fragmented fringe**: tech giants and established pure-plays (Microsoft, Okta/Auth0, Ping Identity) capture dominant enterprise market share, while emerging sub-segments (B2B SaaS auth, passkeys, non-human/agent identities, and open-source self-hosting) remain highly competitive and fragmented across specialized innovators.



## SaaS/Hosted Platforms

| Company / Product | Size / Valuation (Descending) | Starting Tier Pricing | Free Tier / Trial Limits | Key Features & Focus |
| :--- | :--- | :--- | :--- | :--- |
| **[Microsoft Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)** | **~$3.94T Market Cap** (Microsoft parent; $20B+ annual security business) | **$6.00 / user / month** (Entra ID P1, billed annually) | **Permanent free tier** included with Azure/M365 accounts; capped at 50,000 directory objects (expandable to 300,000 objects with verified custom domain), Security Defaults MFA only, no SLA, and no Conditional Access. | Ubiquitous enterprise cloud identity tightly integrated with Azure, Office 365, and Windows; conditional access and governance. |
| **[Okta](https://www.okta.com/)** | **~$33B Market Cap** (~$2.9B ARR) | **$6.00 / user / month** (Starter Suite; requires $1,500/year contract minimum) | **30-day free trial**; includes access to workforce identity features and Okta Workflows capped at 5 active flows and 2 million step executions during the trial. | Enterprise workforce identity leader with universal directory, SSO, adaptive MFA, lifecycle management, and governance. |
| **[Auth0 (Okta)](https://auth0.com/)** | **$6.5B Acquisition Valuation** (acquired by Okta; part of Customer Identity Cloud) | **$35.00 / month** (B2C Essentials up to 500 MAUs) / **$150.00 / month** (B2B Essentials up to 500 MAUs) | **Permanent free tier** up to **25,000 Monthly Active Users (MAUs)**; includes unlimited social logins, passwordless/passkeys, up to 5 organizations, and 1 custom domain (no custom DB or separate dev/prod environments). | Developer-friendly CIAM with extensible Actions/Rules, deep SDK ecosystems, and seamless social/enterprise auth. |
| **[Ping Identity (ForgeRock)](https://www.pingidentity.com/)** | **$2.8B Acquisition Valuation** (combined with ForgeRock by Thoma Bravo; ~$800M ARR) | **$3.00 / user / month** (PingOne Workforce Essential, 5,000-user minimum) / **$35,000 / year** (PingOne Customer Essential base package) | **30-day free trial**; capped at up to 1,000 active identities and 5 sandbox environments with standard rate/messaging limits. | Enterprise-grade workforce and CIAM platform with AI-driven risk scoring, decentralized identity, and hybrid deployment support. |
| **[JumpCloud](https://jumpcloud.com/)** | **$2.6B Valuation** (Series F; ~$150M–$200M ARR) | **$9.00 / user / month** (Device Management, billed annually) / **$11.00 / user / month** (SSO bundle, billed annually) | **30-day free trial** for new sign-ups with full-platform access; permanent free tier was discontinued for accounts created after Feb 1, 2024. | Cloud Directory-as-a-Service uniting cross-OS device management (MDM), LDAP/Radius, and SSO for SMBs and mid-market teams. |
| **[WorkOS](https://workos.com/)** | **$2.0B Valuation** (Series C; ~$30M ARR) | **$125.00 / connection / month** (SSO 1–15 connections; Directory Sync/SCIM billed separately at $125/connection/month) | **Permanent free tier** for core auth (AuthKit) up to **1,000,000 Monthly Active Users (MAUs)**; includes user management, social auth, MFA, passkeys, and free staging environments (enterprise SSO/SCIM require paid connections). | Developer platform designed specifically for B2B SaaS enterprise readiness (Enterprise SAML/OIDC SSO, SCIM Directory Sync, and Admin Portals). |
| **[OneLogin (One Identity)](https://www.onelogin.com/)** | **~$500M Est. Acquisition Valuation** (acquired by One Identity / Quest Software; ~$60M estimated ARR) | **$4.00 / user / month** (Advanced Plan, billed annually) | **30-day free trial**; includes full access to Cloud Directory, desktop/mobile SSO, MFA, VPN integration, and standard security reporting policies. | Cloud SSO and identity management providing directory sync, smart MFA, and workforce provisioning across enterprise SaaS suites. |



## Open-Source GitHub Projects



- **[Keycloak](https://github.com/keycloak/keycloak)**  

  **The open-source IAM standard.** Red Hat-backed, CNCF project with **25K+ GitHub stars** and the broadest protocol support: OIDC, OAuth 2.0, SAML 2.0, and LDAP federation . **Strengths**: closest feature parity to commercial platforms like ForgeRock or Ping Identity; mature clustering and identity brokering; huge community and documentation. **Trade-offs**: Java/Quarkus stack is resource-heavy; **theming and UX customization are notoriously painful** relative to modern alternatives; operational burden for upgrades and clustering . Best for enterprises that need comprehensive, standards-complete IAM and have Java/ops expertise to run it.



- **[Authentik](https://github.com/goauthentik/authentik)**  

  **The modern alternative with better ergonomics.** Python-based, container-native IdP with a **visual flow engine** for designing custom authentication workflows by chaining stages and policies . **Key differentiators**: markedly better admin UX and theming than Keycloak; supports OIDC, SAML, LDAP outpost, proxy auth, and RADIUS outpost; MIT core with commercial enterprise features . **Trade-offs**: smaller community and ecosystem than Keycloak; younger project . Best for teams that want self-hosted IAM with modern UX and are willing to accept a smaller ecosystem in exchange for better ergonomics.



- **[Ory (Kratos / Hydra / Keto / Oathkeeper)](https://github.com/ory)**  

  **The composable, headless building blocks.** Ory provides separate components for identity management (Kratos), OAuth 2.0/OIDC server (Hydra), authorization (Keto), and access proxy (Oathkeeper) . **Key differentiator**: API-first architecture gives complete control over the user experience—you build the UI, Ory handles the security-critical backend. **Trade-offs**: more assembly required than monolithic IdPs; you must build the UX layer yourself . Best for engineering teams that want headless, composable identity primitives for microservices and custom auth experiences.



- **[Zitadel](https://github.com/zitadel/zitadel)**  

  **The cloud-native multi-tenant IdP.** Go-based, AGPL-3.0 licensed, with **native multi-tenancy** (instances and organizations) and an **event-sourced architecture** for full audit trails . Supports OIDC, SAML, passwordless (passkeys/biometrics), and actions for custom logic. **Trade-offs**: smaller ecosystem and fewer pre-built integrations than incumbents; AGPL license may matter for some commercial deployments . Best for B2B SaaS products that need multi-tenancy out of the box and teams wanting the OSS-or-managed choice.



- **[Authelia](https://github.com/authelia/authelia)**  

  **The reverse-proxy authentication specialist.** Go-based, designed to sit in front of web applications as a **forward-auth middleware** for Traefik, Nginx, Caddy, and Envoy . Provides SSO, MFA (TOTP, WebAuthn, Duo), and fine-grained access policies. **Limitation**: limited or no SAML support; not a full IdP—it's an authentication portal . Best for homelabs and self-hosted environments that need to protect services behind a reverse proxy without deploying a full IdP.



- **[Casdoor](https://github.com/casdoor/casdoor)**  

  **The Go-based alternative with built-in MCP server.** Apache-2.0 licensed, with support for OAuth 2.0/OIDC, SAML, CAS, LDAP server, RADIUS server, and **MCP server with OAuth 2.1** for AI agent authentication . Supports 70+ social/enterprise providers including WeChat, DingTalk, and Lark . **Trade-offs**: smaller community than Keycloak; less mature enterprise tooling. Best for teams wanting a Go-based IdP with broad protocol support and AI/MCP integration.



### Additional Strong Open-Source Options



- **FusionAuth** — Java-based CIAM platform with a polished out-of-the-box UI and a free self-hosted Community Edition. Best for teams wanting a commercial-grade CIAM experience with an open-source core .

- **SuperTokens** — Open-source auth with a focus on frontend flexibility and custom UX. Best for full-stack teams wanting to own the auth UI without building the backend from scratch .

- **WSO2 Identity Server** — Java-based, Apache 2.0, with deep API management integration. Best for enterprises already in the WSO2 ecosystem .

- **Gluu/Janssen** — Linux Foundation-backed IAM platform with strong federation capabilities. Best for organizations needing a community-governed alternative to Red Hat-backed Keycloak .

- **Frameworks for building custom systems**: Use **Keycloak** as the enterprise IdP when broad protocol support and maturity matter most. Choose **Authentik** when you want modern UX and a flexible flow engine. Use **Ory** when you need headless, composable identity for microservices and will build the UI yourself. Use **Zitadel** for multi-tenant B2B SaaS. Use **Authelia** for reverse-proxy protection in homelab/small-team environments.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Self-hosted IAM shifts operational burden to you**: authentication is security-critical infrastructure. Plan for high availability, backup strategies, upgrade cadence, and security patching—Keycloak's operational burden is a commonly cited reason teams migrate away .

- **License matters**: Keycloak and Casdoor are Apache 2.0; Zitadel is AGPL-3.0; Authentik is MIT core with commercial enterprise features. Verify license compatibility before deploying in commercial products .

- **No single solution is universally best**: Keycloak leads in features and community; Authentik in UX; Ory in flexibility; Zitadel in multi-tenancy. Match the tool to your team's skills and your application's requirements .



---



**Made for platform engineers, security architects, and developers building authentication infrastructure.**  

Let's make identity management more open, understandable, and appropriately scoped.
