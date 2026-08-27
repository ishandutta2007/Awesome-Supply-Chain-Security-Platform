# Awesome-Supply-Chain-Security-Platform

Edit
Top Supply Chain Security Platforms Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Software Supply Chain Security, SCA, SBOM, Malware Detection, Provenance & Software Integrity
Last updated: August 2026

This repository tracks notable SaaS/hosted platforms and open-source projects for Software Supply Chain Security. These tools help organizations discover, analyze, secure, and continuously monitor software dependencies, open-source packages, containers, build pipelines, artifacts, CI/CD systems, and third-party software.

Software supply chain security covers areas including software composition analysis (SCA), dependency risk, malicious-package detection, SBOM generation and analysis, vulnerability management, license compliance, artifact provenance, build integrity, package signing, dependency confusion, typosquatting, compromised maintainer detection, secrets, CI/CD security, and supply-chain attack-path analysis.

Examples include Chainguard, Socket, Phylum, Apiiro, OX Security, Snyk, Mend.io, Anchore, JFrog Xray, and Google Assured OSS — spanning trusted software distribution, SCA, malicious-package detection, SBOM management, software factory security, and dependency risk management. Gartner's 2026 Software Supply Chain Security Magic Quadrant also identifies the category as an emerging standalone market.

Open-source emphasis: This list heavily emphasizes open-source projects that can be self-hosted, integrated into CI/CD, embedded into developer workflows, or used to build a complete software supply-chain security stack. Important projects include Sigstore, SLSA, GUAC, OSV-Scanner, OpenSSF Scorecard, in-toto, Syft, Grype, Trivy, Dependency-Track, Dependency-Check, Cosign, and Gitsign. Sigstore provides open-source signing and verification infrastructure, while GUAC aggregates SBOM and supply-chain metadata into a graph for security analysis.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites or canonical GitHub repositories.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

Open-Source Building Blocks

Typical Open-Source Architecture

Key Capabilities to Evaluate

How to Contribute

Disclaimer

## SaaS/Hosted Platforms

| Platform | Focus & Description | Starting Pricing | Free Tier / Free Trial Limits |
| :--- | :--- | :--- | :--- |
| **Chainguard** | Hardened, minimal, continuously maintained container images, OS packages, and verifiable SLSA provenance built from source in hardened infrastructure. | Starts at **$19,000/year** (Catalog tier for a team of 10 with contractual CVE remediation SLAs; custom per-image pricing also available). | **Catalog Starter (Free forever):** Access to 5 fixed container images for production use (no CVE SLA; requires business email). |
| **Socket** | Proactive detection of malicious packages, install scripts, typosquatting, and supply chain threats across npm, PyPI, and Go ecosystems. | **Team plan:** Starts at **$25/developer/month** ($300/dev/year billed annually). | **Free tier forever:** 1,000 scans/month, 500 API calls/hour, up to 3 team members, 1 repo label. 100% free with unlimited scans for public open-source repos. |
| **Phylum** | Automated software supply chain security analyzing open-source dependencies for malicious code, author reputation anomalies, and software risks. | **Enterprise plans:** Annual contracts typically starting at **$5,000–$10,000/year** based on developer count (acquired by Veracode). | **Free Trial only:** 14 to 30-day enterprise evaluation / Proof of Concept (POC) upon sales contact. (Community Edition sunset in Feb 2025). |
| **Apiiro** | Application Security Posture Management (ASPM) and software supply chain security providing code-to-cloud risk graph, secrets, and reachability. | **Enterprise plans:** Starts at **$15,000–$25,000/year** via AWS Marketplace / direct contracts based on contributing developer count. | **Free Trial only:** 14-day free trial for Apiiro Guardian Agent on GitHub Marketplace; 14-day guided enterprise platform evaluation. |
| **OX Security** | Pipeline security and ASPM offering pipeline attack-path analysis, Pipeline-Bill-of-Materials (PBOM), and software supply chain risk visibility. | **Enterprise plans:** Custom annual contracts starting at **$12,000–$20,000/year** depending on developer count / AWS Marketplace private offers. | **Free Trial only:** 14 to 30-day complimentary full-access trial / Proof of Concept upon demo request (includes full automated workflow features). |
| **Snyk** | Developer security platform providing open-source dependency scanning (SCA), SAST (Snyk Code), container security, and IaC scanning. | **Team plan:** Starts at **$25/contributing developer/month** (minimum 5 developers = $125/month). | **Free tier forever:** 400 Open Source (SCA) tests/month, 100 Code (SAST) tests/month, 300 IaC tests/month, 100 Container tests/month. |
| **Mend.io** | Application security platform providing SCA, open-source license compliance, automated dependency updates (Renovate), and supply chain defense. | **Enterprise plans:** Starts at **$12,000–$15,000/year** (or ~$250–$600/developer/year depending on product bundle). | **Mend Bolt (Free forever):** Free vulnerability scans for GitHub and Azure DevOps repos; free Renovate for OSS repos; 14-day free trial for enterprise platform. |
| **Anchore** | Cloud-native software supply chain security platform focused on SBOM generation, container security, vulnerability analysis, and policy enforcement. | **Enterprise plans:** Base policy packages start at **$5,000/year** on AWS Marketplace; full platform contracts scale with container volume. | **Free Trial only:** 15-day free trial for Anchore Enterprise in AWS / cloud environments (in addition to open-source Syft and Grype tools). |
| **JFrog Xray** | Universal artifact analysis and binary SCA platform integrated with JFrog Artifactory for deep vulnerability and license scanning across package ecosystems. | **Cloud Pro:** Starts at **$150/month** (promotional rates from $50/month) including 25 GB monthly consumption ($1.25/GB overage). | **Cloud Free tier forever:** 2 GB storage and 10 GB data transfer per month, with access to core artifact repository and Xray vulnerability scanning. |
| **Google Assured OSS** | Curated open-source packages (Java, Python, Go) verified, built from source, vulnerability-checked, and signed with SLSA provenance by Google. | **Free for Standard tier;** **Premium tier:** Included with Security Command Center Premium (starts at **$0.0057/vCPU-hour** or 20% Assured Workloads fee). | **Free tier forever:** Access to 2,500+ curated OSS packages with security metadata and SBOMs at $0/month; new GCP accounts receive $300 free trial credits (90 days). |
| **GitHub Advanced Security** | Developer security incorporating CodeQL code scanning, secret scanning with push protection, Dependabot, and supply chain dependency review. | **Secret Protection:** **$19/active committer/month**; **Code Security:** **$30/active committer/month** (or $49/committer/month bundle for GitHub Enterprise). | **Free tier forever for public repositories:** Unlimited secret scanning, push protection, CodeQL code scanning, and Dependabot alerts/PRs on GitHub.com. |
| **Black Duck** | Application security platform with extensive software composition analysis (SCA), open-source risk management, license compliance, and SBOM capabilities. | **Enterprise plans:** Contracts typically start at **$10,000–$20,000/year** based on codebase volume and developer count. | **Free Trial only:** 30-day Proof of Concept (POC) / trial upon sales consultation and demo request. |
| **Sonatype Nexus Lifecycle** | SCA and repository firewall policy enforcement powered by Nexus Intelligence to block malicious components and govern dependencies. | **Enterprise plans:** Typically starts at **$810/developer/year** for platform bundles; entry contracts start around ~$10,000/year. | **Free Trial only:** 14-day free trial for Sonatype Lifecycle platform (plus free open-source Nexus Repository OSS). |
| **Checkmarx** | Application security platform (Checkmarx One) integrating SCA, supply chain security, SAST, API security, and container image analysis. | **Enterprise plans:** Starts at **$20,000–$30,000/year** depending on developer seats and selected modules. | **Checkmarx Developer Assist:** Free IDE plugin tier; **Checkmarx One:** 14 to 30-day guided evaluation Proof of Concept (POC) upon request. |
| **Endor Labs** | Application and software supply chain security platform focused on dependency intelligence, reachability analysis, and risk prioritization. | **Enterprise plans:** Custom annual contracts starting at **$15,000/year** based on developer count via direct sales / AWS Marketplace. | **AURI for Developers (Free forever):** Local developer security scanning (SAST, SCA, secrets, malware) via CLI/MCP with no time limit or credit card required. |
| **FOSSA** | Open-source management and SCA platform focused on dependency security, license compliance, SBOMs, and open-source governance. | **Business plan:** Starts at **$20/developer/month** (billed annually); Enterprise plans custom quoted. | **Free plan forever:** Up to 5 projects and 10 contributing developers with full open-source license & vulnerability scanning. |
| **Cycode** | ASPM platform providing visibility and security controls across source code, CI/CD pipelines, hardcoded secrets, and developer environments. | **Enterprise plans:** Custom annual subscription starting at **$10,000–$15,000/year** on AWS/Azure Marketplace based on developer count. | **Free Trial only:** 14-day free trial upon request (full platform access including hardcoded secret detection and pipeline security). |
| **ReversingLabs** | Binary analysis and software integrity platform (Spectra Assure) inspecting build outputs, containers, and packages for tampering and malware. | **Enterprise plans:** Spectra Assure contracts typically start at **$15,000–$25,000/year** based on artifact scan volume. | **Spectra Assure Community (Free forever):** Free web-based package risk search engine; **14-day free trial** for full Spectra Assure enterprise platform. |
| **Lineaje** | Software supply chain security platform providing software bill of materials (SBOM) management, tamper detection, and multi-tier component risk analysis. | **Enterprise plans:** Private offer contracts on AWS Marketplace typically starting at **$12,000/year**; PAYG options available for SCA360. | **Free Trial only:** 14 to 30-day enterprise Proof of Concept (POC) trial license upon request. |
| **RapidFort** | Cloud-native container attack surface reduction and hardening platform optimizing images, removing unused packages, and monitoring CVEs. | **Platform plans:** Starts at **$5,000/month** (or $75,000/year on AWS Marketplace with unlimited container coverage). | **Community Images (Free forever):** Free pre-hardened container images on GitHub; **30-day free trial license** for full SASM platform. |
| **ActiveState Platform** | Secure language runtime builder and dependency manager for Python, Perl, and Tcl with automated CVE fixes and reproducible builds. | **SMB Tier:** Starts at **$1,200/language/year** (or legacy Team tiers from $84/user/month billed annually). | **Free tier forever:** 1 active runtime project for individual developers with automated build and dependency management. |
| **JFrog Artifactory** | Universal artifact repository and binary management control point for packages, container images, Helm charts, and build metadata. | **Cloud Pro:** Starts at **$150/month** (or $50/month promotional rate) with 25 GB monthly consumption ($1.25/GB overage). | **Cloud Free tier forever:** 2 GB storage and 10 GB data transfer per month. |
| **GitLab** | Integrated DevSecOps platform with dependency scanning, container scanning, secret detection, SBOM generation, and CI/CD security controls. | **Premium:** **$29/user/month**; **Ultimate** (full supply chain security & compliance): **$99/user/month** (billed annually). | **Free tier forever:** Up to 5 users per namespace, 400 CI/CD compute minutes/month, 10 GiB storage, and up to 3 top-level groups. |
| **Azure Defender for DevOps** | Cloud security capability securing multi-pipeline environments (Azure DevOps, GitHub, GitLab) with code, secret, and posture analysis. | **Defender CSPM:** Integrated into Microsoft Defender for Cloud starting at pay-as-you-go resource rates (**$0.0057/vCPU-hour** / server rates). | **Foundational CSPM (Free forever):** Basic DevOps security posture recommendations at $0; **30-day free trial** for enhanced Defender for Cloud capabilities. |
| **AWS CodeArtifact** | Managed artifact repository service for securely storing, publishing, and sharing software packages (npm, PyPI, Maven, NuGet, Cargo, Swift). | **Pay-as-you-go:** **$0.05 per GB-month** of storage and **$0.05 per 10,000 requests** (after free tier allowance). | **AWS Free Tier forever:** 2 GB storage/month and 100,000 requests/month included at no cost. |

Open-Source GitHub Projects
Supply Chain Integrity & Provenance

Sigstore
Open-source ecosystem for signing and verifying software artifacts using identity-based, ephemeral signing mechanisms and transparency logs. It is designed to make artifact signing easier without traditional long-lived key management.

Cosign
Sigstore's open-source container and artifact signing/verification tool. It supports signing container images and other artifacts and verifying their signatures and associated attestations.

SLSA
Open framework for improving software supply-chain integrity through progressively stronger provenance and build-security guarantees.

in-toto
Framework for securing the integrity of software supply chains by recording and verifying metadata about the steps used to produce software.

gitsign
Keyless Git commit signing based on Sigstore infrastructure, enabling identity-based verification of Git history.

gittuf
Open-source project for protecting Git repositories against malicious or unauthorized changes through verifiable repository policies and cryptographic controls.

SBOM Generation & Analysis

Syft
Open-source SBOM generation tool from Anchore that identifies software components in container images, filesystems, and other artifacts.

Grype
Open-source vulnerability scanner for container images, filesystems, and SBOMs. It pairs naturally with Syft for an inventory-to-vulnerability workflow.

Trivy
Comprehensive open-source security scanner covering container images, filesystems, Git repositories, Kubernetes, IaC, dependencies, secrets, and vulnerabilities.

CycloneDX
Open standard and ecosystem for machine-readable SBOMs and software component metadata.

SPDX
Linux Foundation-hosted open standard for software package identification, SBOM representation, licensing, and supply-chain metadata.

Dependency-Track
Open-source platform for continuous SBOM analysis, vulnerability tracking, component risk management, and organization-wide software supply-chain visibility.

OWASP Dependency-Check
Open-source SCA utility that identifies publicly disclosed vulnerabilities in project dependencies.

Vulnerability & Dependency Scanning

OSV-Scanner
Google's open-source vulnerability scanner using the OSV database to identify known vulnerabilities in dependency manifests, lockfiles, SBOMs, and related artifacts.

OSV.dev
Open vulnerability database and infrastructure aggregating vulnerability information across multiple open-source ecosystems.

Trivy
Broad security scanner covering dependencies, containers, Kubernetes, IaC, secrets, and vulnerabilities.

Grype
Fast vulnerability scanner designed to consume SBOMs and scan container images and filesystems.

OWASP Dependency-Check
Dependency vulnerability identification and reporting tool.

OWASP Dependency-Track
Portfolio-level SBOM and vulnerability management platform.

Malicious Package Detection

OpenSSF Package Analysis
OpenSSF project focused on analyzing packages and identifying potentially malicious behavior in open-source ecosystems.

GuardDog
Open-source malicious-package detection tool originally developed by Datadog, using static analysis and heuristics to identify suspicious behavior in packages.

Socket CLI
Open-source CLI components for integrating Socket's package-risk analysis into developer workflows. The broader Socket detection platform remains a hosted commercial service.

Supply Chain Guard
Open-source supply-chain security scanner combining package analysis, malware indicators, SBOM generation, and provenance checks across multiple ecosystems.

Supply Chain Graph & Security Posture

GUAC
Graph for Understanding Artifact Composition. GUAC aggregates SBOMs, attestations, vulnerabilities, provenance, VEX, Scorecard, SLSA, SPDX, CycloneDX, and related metadata into a high-fidelity graph for organizational supply-chain analysis.

OpenSSF Scorecard
Automated assessment of open-source projects based on security practices such as branch protection, dependency management, code review, and workflow security.

Minder
OpenSSF project for continuously evaluating and enforcing security policies across software repositories and development workflows.

Trustify
Open-source software supply-chain security infrastructure for aggregating, querying, and analyzing SBOM and vulnerability information.

Secrets & Repository Security

Gitleaks
Open-source secret scanner for detecting credentials and sensitive information in Git repositories and CI/CD workflows.

TruffleHog
Secret-scanning platform capable of searching Git repositories, filesystems, and other sources for credentials and sensitive secrets.

GitGuardian Hashed Git
Open-source CLI for secret detection integrated into developer and CI workflows; the broader GitGuardian platform is commercial.

Container & Artifact Security

Trivy
Multi-purpose scanner covering containers, Kubernetes, filesystems, repositories, dependencies, secrets, and configuration.

Clair
Open-source vulnerability analysis service for container images.

Notary Project
Open-source ecosystem for signing and verifying software artifacts and container images.

Notation
CNCF Notary Project implementation for signing and verifying OCI artifacts.

Cosign
Keyless artifact signing and verification using Sigstore.

Additional Strong Open-Source Options

GUAC — Software supply-chain knowledge graph.

Sigstore — Artifact signing, verification, and transparency.

Cosign — Container and artifact signing.

SLSA — Build integrity and provenance framework.

in-toto — End-to-end supply-chain integrity.

gittuf — Git repository integrity.

OpenSSF Scorecard — Open-source project security posture.

Minder — Policy-driven security posture management.

OSV-Scanner — Dependency vulnerability scanning.

OSV.dev — Open vulnerability intelligence.

Syft — SBOM generation.

Grype — SBOM and vulnerability scanning.

Trivy — Comprehensive artifact and dependency scanning.

Dependency-Track — Enterprise SBOM analysis.

Dependency-Check — Dependency vulnerability analysis.

GUAC — Supply-chain metadata correlation.

Package Analysis — Malicious package analysis.

GuardDog — Heuristic package malware detection.

Gitleaks — Secret detection.

TruffleHog — Credential and secret discovery.

Clair — Container vulnerability analysis.

Notary Project — Artifact signing and verification.

CycloneDX — SBOM standard and tooling.

SPDX — SBOM and license standard.

Open-Source Building Blocks
Layer	Open-Source Options	Purpose
Artifact Signing	Sigstore, Cosign, Notation	Sign and verify software artifacts
Build Provenance	SLSA, in-toto	Establish trustworthy build provenance
Git Integrity	gittuf, gitsign	Protect source repositories and commits
SBOM Generation	Syft, CycloneDX, SPDX	Inventory software components
SBOM Management	Dependency-Track, GUAC	Centralize and analyze software composition
Vulnerability Scanning	OSV-Scanner, Grype, Trivy, Dependency-Check	Detect known vulnerabilities
Malware Detection	Package Analysis, GuardDog, Supply Chain Guard	Identify suspicious packages
Container Security	Trivy, Clair, Grype	Scan images and container artifacts
Supply-Chain Graph	GUAC	Correlate SBOM, provenance and vulnerability data
Project Security	OpenSSF Scorecard	Evaluate upstream security practices
Policy Enforcement	Minder	Apply security policies to repositories/workflows
Secrets	Gitleaks, TruffleHog	Detect credentials and secrets
Artifact Registry	Harbor	Self-hosted container registry with security controls
Container Signing	Cosign, Notation	Cryptographically verify artifacts
Package Security	OSV.dev	Open vulnerability intelligence
Metadata	VEX, SPDX, CycloneDX	Communicate component security status
Observability	OpenTelemetry	Trace software build/security workflows
CI/CD	GitHub Actions, GitLab CI, Tekton	Integrate security gates into pipelines
Storage	PostgreSQL, MinIO	Store supply-chain metadata and artifacts
Analytics	ClickHouse, PostgreSQL	Analyze SBOM and security events
Dashboards	Grafana	Visualize security posture and pipeline telemetry
Typical Open-Source Supply Chain Security Architecture

A company seeking to build a self-hosted alternative to commercial supply-chain security platforms can combine:

Git repositories — Source code and dependency manifests.

OpenSSF Scorecard — Evaluate upstream project security posture.

OSV-Scanner — Scan dependency trees against known vulnerabilities.

Syft — Generate SBOMs from source trees, binaries, and container images.

Grype / Trivy — Scan SBOMs and artifacts for vulnerabilities.

Package Analysis / GuardDog — Detect suspicious or malicious package behavior.

Gitleaks / TruffleHog — Detect leaked credentials.

SLSA + in-toto — Generate and verify build provenance.

Sigstore + Cosign — Sign and verify artifacts.

GUAC — Correlate SBOMs, provenance, vulnerabilities, VEX, and project metadata.

Dependency-Track — Maintain organization-wide SBOM and vulnerability visibility.

Minder — Apply policy and continuously evaluate security posture.

Harbor — Store and manage trusted container artifacts.

Kubernetes — Run the security platform at scale.

Grafana + Prometheus — Monitor security pipelines and infrastructure.

This architecture can provide a highly customizable, self-hosted software supply-chain security platform covering source → dependency → build → artifact → registry → deployment.

Commercial Platform vs Open-Source Stack
Capability	Commercial Platform	Open-Source Stack
Dependency discovery	Built-in	OSV-Scanner / Syft / ecosystem tooling
SCA	Built-in	Grype / Trivy / Dependency-Check
SBOM generation	Built-in	Syft / CycloneDX / SPDX
SBOM management	Built-in	Dependency-Track / GUAC
Malware detection	Advanced vendor engines	Package Analysis / GuardDog / custom analysis
Provenance	Usually integrated	SLSA + in-toto
Artifact signing	Integrated	Sigstore + Cosign
Container scanning	Integrated	Trivy / Grype / Clair
License compliance	Usually integrated	SPDX / FOSSology / custom policy
Supply-chain graph	Increasingly common	GUAC
Developer UX	Highly integrated	Requires assembly
CI/CD integration	Built-in	GitHub/GitLab/Jenkins/Tekton integrations
Policy engine	Built-in	Minder / custom policy
Threat intelligence	Vendor-maintained	OSV + community databases
Zero-day / malware research	Often vendor-operated	Requires building/combining tooling
Self-hosting	Usually limited	Strong
Customization	Moderate	Very high
Data ownership	Vendor-dependent	Organization-controlled
Maintenance	Vendor-managed	Organization-managed
Total engineering effort	Lower	Higher
Transparency	Vendor-dependent	Code-level transparency
Key Capabilities to Evaluate

When comparing software supply chain security platforms, evaluate:

Software Composition Analysis (SCA)

Dependency discovery

Direct and transitive dependency analysis

Reachability analysis

Known vulnerability detection

Malicious package detection

Typosquatting detection

Dependency confusion detection

Package reputation

Maintainer risk

Package behavior analysis

Install-script analysis

Post-install behavior

Network behavior

Credential-access behavior

SBOM generation

SBOM ingestion

SBOM normalization

CycloneDX

SPDX

VEX

OpenVEX

Software provenance

SLSA

in-toto

Artifact signing

Sigstore

Container signing

Container vulnerability scanning

Binary analysis

CI/CD security

GitHub/GitLab integration

Package registry security

Artifact repository security

Open-source license compliance

License policy enforcement

Secrets detection

Build integrity

Reproducible builds

Dependency pinning

Dependency update automation

Security posture scoring

OpenSSF Scorecard

Supply-chain attack-path analysis

Software inventory

Developer risk prioritization

Policy-as-code

Runtime monitoring

Kubernetes security

Cloud-native security

AI/ML dependency security

Model artifact security

Audit trails

Compliance reporting

Self-hosting

API access

Webhooks

CLI integration

IDE integration

How to Contribute

Fork the repo.

Add/edit entries in README.md following the existing format.

Include: name, link, 1–2 sentence description, and whether it is SaaS, hosted, open-source, open-core, or source-available.

For GitHub projects, prefer the canonical upstream repository.

Clearly distinguish complete supply-chain security platforms from SCA scanners, SBOM tools, signing systems, vulnerability databases, and supporting infrastructure.

Verify the current license and repository activity before labeling a project as open source.

Mention supported ecosystems such as npm, PyPI, Maven, Go, Cargo, NuGet, RubyGems, Docker/OCI, and OS packages where applicable.

Mention standards such as SLSA, in-toto, SPDX, CycloneDX, VEX, OpenVEX, and OpenRTB where relevant.

Submit a PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

Commercial supply-chain security platforms frequently change product names, ownership, packaging, and capabilities.

SCA, SBOM management, artifact security, package malware detection, provenance, signing, and supply-chain security platforms are related but distinct categories.

The open-source ecosystem is fragmented across these individual capabilities rather than dominated by a single comprehensive open-source platform.

Some projects listed here are building blocks rather than complete enterprise-grade supply-chain security platforms.

Always verify the current license before deploying or redistributing software.

Open source, source-available, free software, and free hosted tiers are different concepts.

Commercial products may combine proprietary threat intelligence, package telemetry, malware research, behavioral analysis, and managed services that are difficult to reproduce entirely with open-source tooling.

A self-hosted supply-chain security stack requires substantial work around vulnerability intelligence, malware research, provenance verification, policy enforcement, scalability, alert triage, data retention, and operational security.

Software supply chains should be assessed across the complete lifecycle: source → dependency → build → artifact → registry → deployment → runtime.

Security tooling should be integrated into developer workflows without unnecessarily blocking legitimate development.

Made for software engineers, DevSecOps teams, application security teams, platform engineers, CISOs, open-source maintainers, and organizations building secure software factories.
Let's make software supply chains more transparent, verifiable, resilient, developer-friendly, and open-source.
