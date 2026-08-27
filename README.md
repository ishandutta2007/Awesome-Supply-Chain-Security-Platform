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

SaaS/Hosted Platforms

Chainguard
Software supply chain security platform focused on hardened, minimal, continuously maintained software artifacts, containers, libraries, OS packages, CI/CD actions, and verifiable provenance. Chainguard builds artifacts from source in hardened infrastructure and provides policy-controlled repositories.

Socket
Software supply chain security platform specializing in proactive detection of malicious and suspicious behavior in open-source packages, including dependency and package-level risks that may not yet have published CVEs.

Phylum
Software supply chain security platform focused on detecting malicious packages, dependency threats, suspicious package behavior, and emerging attacks across open-source ecosystems.

Apiiro
Application and software supply chain security platform providing code risk visibility, dependency analysis, security posture management, and prioritization across development environments.

OX Security
Software supply chain security platform providing application security posture management, risk correlation, attack-path analysis, and security visibility across the software development lifecycle.

Snyk
Developer security platform providing open-source dependency scanning, container security, IaC security, code security, license analysis, and automated remediation.

Mend.io
Application security platform providing software composition analysis, open-source license compliance, dependency management, supply-chain security, and automated remediation.

Anchore
Cloud-native software supply chain security platform focused on SBOMs, container security, vulnerability analysis, policy enforcement, and secure software delivery.

JFrog Xray
Continuous software composition and artifact analysis platform integrated with JFrog's software supply chain. Xray supports source and binary SCA across numerous package ecosystems, operating-system packages, containers, and other artifact types.

Google Assured OSS
Google Cloud service providing curated open-source packages with security metadata, SBOMs, vulnerability remediation, and signed provenance. Google currently describes the service as covering 2,500+ curated Java and Python packages.

GitHub Advanced Security
Developer security platform incorporating dependency graph analysis, Dependabot, secret scanning, code scanning, dependency review, and software supply-chain security capabilities.

Black Duck
Application security platform with extensive software composition analysis, open-source risk management, vulnerability identification, license compliance, and SBOM capabilities.

Sonatype Nexus Lifecycle
Software composition analysis and repository security platform providing dependency intelligence, policy enforcement, license compliance, and vulnerability management.

Checkmarx
Application security platform spanning SCA, SAST, IaC, API security, and software supply chain security.

Endor Labs
Application and software supply chain security platform focused on dependency intelligence, reachability analysis, dependency lifecycle management, and risk prioritization.

FOSSA
Open-source management and software composition analysis platform focused on dependency security, license compliance, SBOMs, and open-source governance.

Cycode
Application security posture management platform providing visibility and security controls across source code, CI/CD, identities, dependencies, and developer environments.

ReversingLabs
Software supply chain security and malware analysis platform specializing in binary analysis, malicious-package detection, artifact intelligence, and software integrity.

Lineaje
Software supply chain security platform providing software bill of materials management, software composition analysis, supply-chain intelligence, and risk management.

RapidFort
Cloud-native software supply chain security platform focused on securing, reducing, and continuously monitoring container images and their dependencies.

ActiveState Platform
Software supply chain platform focused on securing and managing language runtimes and open-source dependencies with controlled, reproducible builds.

JFrog Artifactory
Universal artifact repository providing a central control point for binaries, packages, containers, and software artifacts; frequently used together with Xray for supply-chain security.

GitLab
DevSecOps platform incorporating dependency scanning, SBOMs, container scanning, vulnerability management, package registries, and CI/CD security controls.

Azure Defender for DevOps
Microsoft cloud security capabilities integrating DevOps repositories and pipelines with vulnerability, dependency, secret, and security posture analysis.

AWS CodeArtifact
Managed artifact repository for storing and consuming software packages across supported language ecosystems, useful as a controlled distribution point within secure software supply chains.

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
