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

## Cybersecurity

## Data

## Misconception in My Track

## Open Question
