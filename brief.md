Version: NAFATH-V4

Track: Cybersecurity

## Overview

A national service provider relies on secure software, artificial intelligence, mobile applications, networks, cybersecurity practices, and trustworthy data to deliver reliable digital services. Each area introduces risks that can affect the others. Secure software configuration protects credentials and other sensitive settings from exposure. AI security considers attacks that manipulate model inputs or training data. Mobile security verification helps identify weaknesses before applications are released. Network security helps detect route manipulation and protect traffic from interception. Cybersecurity teams investigate vulnerabilities, assess their impact, and apply effective mitigations. Data transparency, including software bills of materials, helps organisations understand the components and dependencies in their systems. Together, these practices support a more resilient service by improving visibility, verification, and coordinated risk management across the software supply chain.

## Software

The Twelve-Factor App recommends keeping deployment-specific configuration separate from application code. This includes database connection details, service credentials, and hostnames, which can change between environments. Environment variables provide a standard way to supply these values without hard-coding them in the repository. Separating configuration from code reduces the risk of accidentally exposing secrets when code is shared and makes the same application easier to deploy across different environments.

Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI

Two important adversarial machine-learning attack types are evasion and poisoning. In an evasion attack, an attacker changes an input at inference time so a trained model makes an incorrect prediction, without necessarily changing its training data. In a poisoning attack, an attacker contaminates training data or otherwise influences the training process, aiming to make the resulting model behave incorrectly. The distinction is whether the attack targets model use or model training.

Resource: Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://www.nist.gov/publications/adversarial-machine-learning-taxonomy-and-terminology-attacks-and-mitigations-0

## Mobile

The OWASP Mobile Application Security Verification Standard (MASVS) defines security requirements for mobile applications. It covers areas such as secure storage, cryptography, authentication, network communication, platform interaction, code quality, resilience, and privacy. Development teams can use these requirements as a checklist to plan security tests and assess whether an application meets expected controls. MASVS helps structure verification; teams should combine it with appropriate testing guidance and evidence rather than treating it as an automatic security guarantee.

Resource: OWASP MASVS - https://mas.owasp.org/MASVS/

## Networking

BGP (Border Gateway Protocol) allows networks to exchange information about internet routes. In a BGP route hijacking attack, an organisation or attacker announces incorrect routing information, which may redirect traffic through an unintended network or make services unreachable. Resource Public Key Infrastructure (RPKI) helps validate whether an autonomous system is authorised to originate a particular IP address prefix. However, RPKI does not encrypt traffic or prevent every routing attack, so it must be combined with other network security measures.

Resource: RIPE NCC - Resource Public Key Infrastructure (RPKI) - https://www.ripe.net/manage-ips-and-asns/resource-management/rpki/ 

## Cybersecurity

Log4Shell is a critical vulnerability identified as CVE-2021-44228 in Apache Log4j, a widely used Java logging library. Under vulnerable configurations, an attacker could exploit specially crafted input to trigger remote code execution, potentially gaining control over an affected system. Its widespread use made identifying vulnerable applications and dependencies particularly important. Organisations should follow vendor guidance, update affected Log4j versions to fixed releases, and verify that vulnerable components are no longer present or exposed.

Resource: CISA - Apache Log4j Vulnerability Guidance - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Data

A Software Bill of Materials (SBOM) is a structured inventory of software components and their relationships within a product. It helps organisations identify dependencies and assess which systems may be affected when a vulnerability is discovered. The NTIA identifies minimum elements including supplier name, component name, component version, other unique identifiers, dependency relationships, SBOM author, and timestamp. Maintaining an accurate SBOM improves transparency and supports vulnerability response, but it does not by itself guarantee that software is secure.

Resource: NTIA - Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

## Misconception in My Track

A common misconception in cybersecurity is that installing a security patch on one system automatically removes a vulnerability from an entire organisation. In reality, vulnerable software may exist in multiple applications, servers, containers, or third-party dependencies. For Log4Shell, security teams must identify affected assets, update vulnerable Log4j components to fixed versions, and verify that remediation is complete. They should also follow relevant vendor and government guidance. CISA's Apache Log4j Vulnerability Guidance explains mitigation actions, showing why vulnerability management requires identification and verification rather than assuming one update protects every system.

Resource: CISA - Apache Log4j Vulnerability Guidance - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Open Question

How can organisations reliably identify every application and third-party dependency affected by a newly discovered vulnerability such as Log4Shell when their software inventories are incomplete or outdated?
