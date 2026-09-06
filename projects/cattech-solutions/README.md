# CatTech Solutions

CatTech Solutions is a fictional technology company created as my first cybersecurity homelab project.

The objective of this project is to design, build and secure a small corporate environment where I can practice cybersecurity concepts in a controlled environment.

## Company Profile

CatTech Solutions is a fictional technology company focused on software development and technical services.

The company has approximately 40–50 employees distributed across the following departments:

- Development
- Technical Support
- IT
- Finance
- Human Resources
- Management

## Main Goals

- Design a realistic small corporate network.
- Configure network segmentation.
- Deploy Active Directory.
- Create users, groups and access permissions.
- Deploy internal corporate services.
- Perform vulnerability assessments.
- Simulate controlled attacks.
- Monitor suspicious activity.
- Apply security hardening and remediation measures.

## Project Phases

### Phase 1 — Corporate Architecture Design

**Status:** In progress

The first phase focuses on designing the corporate infrastructure of CatTech Solutions before deploying any virtual machines.

The current design includes:

- User network
- Server network
- DMZ
- pfSense firewall
- Representative workstations for each department
- Active Directory and DNS server
- File server
- Security monitoring / SIEM server
- Web server in the DMZ

The purpose of this phase is to define the logical structure of the company and establish a clear architecture before implementation.

The current diagram represents only the normal corporate infrastructure of CatTech Solutions.

### Phase 2 — Infrastructure Deployment

**Status:** Planned

This phase will focus on deploying the virtual infrastructure and configuring the network environment.

Planned tasks include:

- Create the required virtual machines.
- Deploy pfSense.
- Configure the internal network segments.
- Assign IP addressing.
- Verify connectivity between authorized network areas.

### Phase 3 — Active Directory Deployment

**Status:** Planned

This phase will focus on deploying and configuring the Windows domain environment.

Planned tasks include:

- Deploy Windows Server.
- Install Active Directory Domain Services.
- Configure DNS.
- Create organizational units.
- Create users and groups.
- Join corporate workstations to the domain.
- Apply basic Group Policy configurations.

### Phase 4 — Corporate Services

**Status:** Planned

This phase will introduce the internal services required by the company.

Planned services include:

- File sharing
- Department-based permissions
- Internal web services
- Security monitoring
- Centralized logging

### Phase 5 — Vulnerability Assessment

**Status:** Planned

The corporate environment will be analyzed to identify security weaknesses and misconfigurations.

The assessment will include:

- Asset discovery
- Port and service enumeration
- Vulnerability scanning
- Risk classification
- Documentation of findings

### Phase 6 — Security Testing

**Status:** Planned

Controlled attacks will be performed inside the isolated laboratory environment.

This phase may include:

- Network reconnaissance
- Service enumeration
- Web application testing
- Credential attacks
- Privilege escalation
- Active Directory security testing

### Phase 7 — Monitoring and Detection

**Status:** Planned

Security monitoring tools will be used to analyze and detect activity generated during the previous phase.

Planned tasks include:

- Collect system logs.
- Monitor authentication events.
- Detect suspicious activity.
- Analyze security alerts.
- Document potential incidents.

### Phase 8 — Hardening and Remediation

**Status:** Planned

Identified vulnerabilities and weaknesses will be remediated.

The environment will then be reassessed to compare its security posture before and after hardening.

## Current Project Status

The project is currently in:

**Phase 1 — Corporate Architecture Design**
