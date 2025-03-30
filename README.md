# SIM/eSIM Security Research

## Overview

This section focuses on the security aspects of SIM cards and eSIM technology, which form the foundation of subscriber identity and authentication in mobile networks.

## Research Tools & Equipment

### Hardware Tools
- [Proxmark3](https://github.com/RfidResearchGroup/proxmark3) - RFID/Smart Card Research Tool
- [ChipWhisperer](https://newae.com/chipwhisperer/) - Side-Channel Analysis Platform
- [ReaderLab](https://github.com/meriac/readerlab) - Open Source Smart Card Reader
- [SIMtrace2](https://osmocom.org/projects/simtrace2/wiki) - SIM Card Protocol Analyzer
- [Smart Card Detective](https://github.com/CardContact/sc-hsm) - Smart Card Testing Device

### Software Tools
- [pySim](https://github.com/osmocom/pysim) - Python Tool for SIM Card Management
- [SIMTester](https://opensource.srlabs.de/projects/simtester) - SIM Card Security Testing Suite
- [Rainbow Tables](https://opensource.srlabs.de/projects/a51-decrypt) - GSM A5/1 Decryption
- [Osmocom SIM Tools](https://osmocom.org/projects/sim-tools/wiki) - Open Source SIM Card Tools
- [CardPeek](https://github.com/L1L1/cardpeek) - Smart Card Analysis Tool

### eSIM Development
- [Open eUICC](https://github.com/estkme-group/openeuicc) - Open Source eSIM Implementation
- [GSMA RSP Test Suite](https://www.gsma.com/esim/rsp-test-suite/) - eSIM Compliance Testing
- [libeuicc](https://source.android.com/docs/core/connect/esim-overview) - Android eSIM Library
- [esim-profiles](https://github.com/estkme-group/esim-profiles) - eSIM Profile Management Tools

## Research Papers & Publications

### SIM Card Security
1. ["Rooting SIM Cards"](https://media.blackhat.com/us-13/us-13-Nohl-Rooting-SIM-cards-Slides.pdf) - Karsten Nohl, BlackHat USA 2013
2. ["The Secret Life of SIM Cards"](https://arxiv.org/pdf/1906.10307.pdf) - USENIX Security 2019
3. ["Practical SIM Card Attacks"](https://www.usenix.org/conference/woot15/workshop-program/presentation/practical-sim-card-attacks) - WOOT'15

### eSIM Security
1. ["Security Analysis of Consumer-Grade eSIM Remote Provisioning"](https://www.blackhat.com/us-20/briefings/schedule/#security-analysis-of-consumer-grade-esim-remote-provisioning-19290) - BlackHat USA 2020
2. ["eSIM Security: Past, Present, and Future"](https://ieeexplore.ieee.org/document/9155619) - IEEE Communications Standards Magazine
3. ["Breaking eSIM Remote Provisioning"](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_f96_paper.pdf) - NDSS 2023

### Side-Channel Analysis
1. ["Power Analysis of SIM Cards"](https://www.iacr.org/archive/ches2002/24230001/24230001.pdf) - CHES 2002
2. ["Practical Template Attacks on SIM Cards"](https://link.springer.com/chapter/10.1007/978-3-030-15462-2_9) - CARDIS 2019

## Educational Videos & Presentations

### Conference Talks
1. ["Hacking SIM Cards with Osmocom"](https://www.youtube.com/watch?v=RZP-EtEXBHk) - CCC 2019
2. ["Breaking eSIM Remote Provisioning"](https://www.youtube.com/watch?v=H4jZ-5h7Hl8) - BlackHat USA 2020
3. ["SIMple: SIM Card Exploitation"](https://www.youtube.com/watch?v=31D94QOo2gY) - DEF CON 21

### Tutorial Series
1. ["Introduction to SIM Card Security"](https://www.youtube.com/watch?v=iJFnYBJJiuQ) - Hak5
2. ["eSIM Technology Deep Dive"](https://www.gsma.com/esim/resources/education/) - GSMA Training
3. ["Smart Card Programming"](https://www.youtube.com/watch?v=9LZXx2pm5xY) - JavaCard Tutorial

## Research Areas

### Physical SIM Security

- **SIM Card Architecture**
  - Smart card hardware security
  - Tamper resistance mechanisms
  - EEPROM/Flash memory security
  - Microcontroller vulnerabilities

- **File System**
  - MF (Master File) structure
  - DF (Dedicated File) access controls
  - EF (Elementary File) content protection
  - File access conditions and permissions

- **Authentication Algorithms**
  - COMP128 (versions and vulnerabilities)
  - Milenage algorithm security
  - TUAK algorithm implementation
  - K₁ encryption key storage and protection

- **SIM Toolkit Applications**
  - STK application vulnerabilities
  - Malicious applet detection
  - S@T Browser security
  - Java Card security boundaries

### eSIM Security

- **Remote Provisioning**
  - SM-DP+ (Subscription Manager - Data Preparation) security
  - SM-SR (Subscription Manager - Secure Routing) vulnerabilities
  - eUICC profile download security
  - LPA (Local Profile Assistant) security

- **Profile Management**
  - Profile switching security
  - Multi-profile coexistence risks
  - Profile deletion verification
  - Operational security for telco profile managers

- **Secure Channel Protocols**
  - SCP03/SCP11 implementation
  - Certificate management
  - Key rotation practices
  - Cryptographic algorithm selection

### Over-The-Air (OTA) Security

- **Update Mechanisms**
  - OTA update authentication
  - SMS-based OTA security
  - CAT_TP security
  - BIP (Bearer Independent Protocol) security

- **Carrier Provisioning**
  - Provisioning message integrity
  - SMS C-Channel security
  - Replay attack prevention
  - OTA command authorization

## Known Vulnerabilities & CVEs

- SIM Card Cloning (CVE-2013-4640)
- Simjacker Vulnerability (CVE-2019-4500)
- WIB Browser Exploit (CVE-2019-4501)
- S@T Browser Attack (CVE-2019-4502)
- OTA Update Bypass (CVE-2021-XXXX)
- eSIM Profile Tampering (CVE-2022-XXXX)
- SIM Toolkit Security Issues (CVE-2020-XXXX)

## Research Methodologies

### Hardware Analysis
- Physical inspection techniques
- Side-channel power analysis
- Timing attack methodology
- Fault injection testing

### Software Analysis
- Logical security testing
- Protocol fuzzing
- Authentication bypass testing
- File system analysis

### eSIM Testing
- Profile management testing
- Remote provisioning analysis
- LPA security assessment
- Certificate validation

## Practical Labs

1. [SIM Card File System Analysis](labs/01-file-system-analysis.md)
   - File structure analysis
   - Access control testing
   - Data extraction techniques

2. [Authentication Algorithm Testing](labs/02-auth-algorithm-testing.md)
   - COMP128 analysis
   - Milenage testing
   - Key extraction attempts

3. [SIM Toolkit Application Security](labs/03-sim-toolkit-security.md)
   - STK app analysis
   - Security boundary testing
   - Applet vulnerability assessment

4. [OTA Security Testing Framework](labs/04-ota-security-testing.md)
   - OTA message analysis
   - Update security testing
   - SMS security assessment

5. [eSIM Profile Management Security](labs/05-esim-profile-security.md)
   - Profile installation testing
   - Security boundary verification
   - Remote management assessment

## Standards & Specifications

### Core Standards
- [ETSI TS 102 221](https://www.etsi.org/deliver/etsi_ts/102200_102299/102221/): Smart Cards; UICC-Terminal interface
- [3GPP TS 31.102](https://portal.3gpp.org/desktopmodules/Specifications/SpecificationDetails.aspx?specificationId=1754): Characteristics of the USIM Application
- [3GPP TS 31.111](https://portal.3gpp.org/desktopmodules/Specifications/SpecificationDetails.aspx?specificationId=1763): USIM Application Toolkit (USAT)
- [GSMA SGP.22](https://www.gsma.com/esim/resources/): RSP Technical Specification

### Security Guidelines
- [NIST SP 800-163](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-163r1.pdf): Mobile App Security Requirements
- [GSMA FS.04](https://www.gsma.com/security/resources/): SIM Security Guidelines
- [Common Criteria](https://www.commoncriteriaportal.org/files/ppfiles/pp0084b_pdf.pdf): Smart Card Protection Profile

## Community Resources

- [SIM Security Wiki](https://simsecurity.org)
- [eSIM Working Group](https://www.gsma.com/esim/workgroup/)
- [TelcoSec SIM Research Forum](https://forum.telco-sec.com/sim)
- [Osmocom SIM Project](https://osmocom.org/projects/sim)
