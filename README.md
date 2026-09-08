# Awesome-Sensitive-Data-Monitoring

## Top Sensitive Data Monitoring Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Data Security Posture Management (DSPM), Sensitive Data Discovery, Classification, Access Intelligence & Data Risk Monitoring*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sensitive Data Monitoring**. These tools discover, classify, and continuously monitor sensitive data (PII, PHI, secrets, regulated data) across cloud, SaaS, on-premises, and structured/unstructured stores to reduce exposure and support compliance.



**Examples** include Varonis, BigID, Microsoft Purview, IBM Guardium, Securiti, Cyera, Sentra, Normalyze, Dig Security, and Ground Labs (the category leaders).



**Open-source emphasis**: Full enterprise DSPM platforms with agentless multi-cloud coverage, continuous posture, and automated remediation are commercial. Open-source options focus on data classification systems, PII discovery scanners, metadata catalogs with auto-classification, secret detection, and redaction toolkits. This section lists every significant relevant project found.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Product | Description | Starting Pricing | Free Tier / Trial Limit |
| :--- | :--- | :--- | :--- |
| **[Varonis](https://www.varonis.com/)** | Data security platform strong in access intelligence, permissions analytics, and monitoring of sensitive data exposure across hybrid environments. | Starting at ~$50 – $95 per user/year (or ~$310/connector/year on AWS Marketplace) | 30-day Free Trial (Data Risk Assessment on full environment) |
| **[BigID](https://bigid.com/)** | Leading data discovery, classification, and privacy platform supporting DSPM, DSAR, and governance across structured and unstructured data. | Starting at ~$25,000/year (~$2,083/month) for entry-level deployments | 30-day Free Trial (Proof of Concept / live evaluation) |
| **[Microsoft Purview](https://www.microsoft.com/en-us/security/business/microsoft-purview)** | Microsoft’s unified data governance suite covering discovery, classification, labeling, DLP, and DSPM capabilities for M365 and Azure. | Starting at $12/user/month (Purview Information Protection add-on) or $0.40/capacity unit hour | 90-day Free Trial (up to 25 user licenses) / 30-day Data Map trial |
| **[IBM Guardium](https://www.ibm.com/products/guardium-data-protection)** | Established data security platform focused on database activity monitoring, vulnerability assessment, and sensitive data protection. | Starting at ~$1,500 per managed server/year (or ~$100,000/year base enterprise tier) | 30-day Free Trial (Guardium Insights SaaS) / 90-day evaluation trial (Guardium Data Protection) |
| **[Securiti](https://securiti.ai/)** | Data command center combining privacy, security, and governance with sensitive data discovery and automation. | Starting at ~$50,000/year base entry (via AWS Marketplace platform contract) | 30-day Free Trial (Proof of Concept / guided environment trial) |
| **[Cyera](https://www.cyera.com/)** | Cloud-native DSPM platform focused on discovering and securing sensitive data across cloud data stores with emphasis on data risk and AI. | Starting at $50,000/year (Standard Package up to 25 TB on AWS Marketplace) | 30-day Free Trial / Proof of Concept (up to 25 TB scanned) |
| **[Sentra](https://www.sentra.io/)** | Cloud-native DSPM solution emphasizing continuous discovery, classification, and protection without moving data out of customer environments. | Starting at $50,000/year (Standard Plan 12-month contract on AWS Marketplace) | 30-day Free Trial / Proof of Concept (full feature evaluation) |
| **[Normalyze](https://normalyze.io/)** | Cloud DSPM platform targeting data posture, exposure detection, and risk prioritization (acquired by Proofpoint). | Starting at $995/month (Premium plan for up to 3 cloud accounts & 1 TB data) | Free forever plan available for 1 cloud account ($0 cost) |
| **[Dig Security](https://www.paloaltonetworks.com/prisma/cloud/dspm)** | Real-time cloud data security posture management (DSPM) and DDR, now integrated into Palo Alto Networks Prisma Cloud. | Starting at ~$18,000/year (~$1,500/month or $90/credit for Prisma Cloud) | 30-day Free Trial (up to 100 cloud workloads / accounts) |
| **[Ground Labs](https://www.groundlabs.com/)** | Specialized sensitive data discovery and scanning tools (Card Recon / Enterprise Recon) for locating regulated data across repositories. | Starting at $1,250 per target/year (Card Recon Desktop & Server) | 7-day Free Trial (Card Recon Desktop scanner) |



## Open-Source GitHub Projects



- **[MDCGS](https://github.com/HaoY-l/mdcgs)**  

  Open-source data classification and grading system that automatically identifies sensitive fields, supports multiple databases, and helps meet data-security compliance requirements with private deployment.



- **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)**  

  Open-source metadata platform with auto-classification workflows (often powered by NLP/spaCy) that can tag PII and other sensitive data as part of broader data governance.



- **[PII / sensitive-data scanners](https://github.com/search?q=PII+discovery+OR+sensitive+data+scan+OR+data+classification)**  

  Community tools and libraries that scan databases, files, and text for personal and regulated data using rules, regex, and ML.



- **[Secret detection tools (gitleaks, detect-secrets, TruffleHog)](https://github.com/gitleaks/gitleaks)**  

  Widely used open-source scanners that find credentials, API keys, and secrets in code and repositories—critical for preventing sensitive data leakage in development pipelines.



- **[Philterd open-source PII toolkit](https://philterd.ai/open-source-software/)**  

  Suite of open-source projects for finding, redacting, monitoring, and auditing PII/PHI in text and streams.



- **[spaCy and NLP-based NER](https://github.com/explosion/spaCy)**  

  Industrial-strength NLP library frequently used as the foundation for custom sensitive-entity detection pipelines.



- **[OpenDLP / MyDLP-style projects](https://github.com/search?q=OpenDLP+OR+MyDLP+OR+data+loss+prevention+open+source)**  

  Classic and community data-loss-prevention and discovery tools focused on scanning endpoints and storage for sensitive content.



- **[Metadata & catalog platforms with classification](https://github.com/search?q=data+catalog+classification+OR+PII+tagging)**  

  Open-source data catalogs that include sensitive-data tagging and policy features.



### Additional Strong Open-Source Options



- **Regular-expression and pattern libraries**: Curated rule sets for common PII, financial, and health identifiers.

- **Database metadata crawlers**: Tools that inventory schemas and sample data for classification.

- **Redaction and masking libraries**: Components that protect sensitive values in logs, outputs, and test data.

- **CI/CD secret scanning**: GitHub Actions and pipeline integrations for continuous secret and PII checks.

- **LLM / GenAI guardrails**: Emerging open-source proxies and filters that prevent sensitive data from being sent to external AI services.

- Policy engines that map classification results to access or retention controls.



**Frameworks for building custom systems**:  

For self-hosted discovery and classification, combine **OpenMetadata** or **MDCGS**-style systems with secret scanners (**gitleaks**, etc.) and NLP libraries (**spaCy**).  

Add redaction toolkits for downstream protection.  

Enterprise-scale, agentless multi-cloud DSPM, continuous posture management, automated least-privilege remediation, and deep access intelligence remain the strength of commercial platforms (Varonis, BigID, Microsoft Purview, Cyera, Sentra, Securiti, IBM Guardium, etc.).  

Many security teams use open-source scanners in development and CI while relying on commercial DSPM for production data estates and compliance reporting.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Sensitive data discovery and monitoring involve highly regulated information. Incorrect classification, incomplete coverage, or improper handling of findings can create legal, privacy, and security risk.

- Open-source tools require careful configuration, tuning of detection rules, and operational processes. They do not automatically satisfy regulatory requirements (GDPR, HIPAA, CCPA, etc.). Organizations remain responsible for the accuracy and completeness of their data security programs.



---



**Made for data security teams, privacy officers, CISOs, data governance leaders, and platform engineers.**  

Let's improve visibility and control over sensitive data through both powerful commercial platforms and transparent open-source building blocks.
