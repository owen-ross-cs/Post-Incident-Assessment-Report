# Post-Incident Assessment Report: National Energy Ransomeware Case Study
a full-scope post-incident audit of a simulated ransomeware attack against a fictional Canadian energy corporation, assessed against ISO/IEC 27001:2022 and SOC 2 Trust Services Criteria. This project demonstrates the end-to-end workflow of a security auditor: reconstructing an attack timeline, identifying control failures, rating risk ans severity, and delivering audit-ready, framework-mapped recommendations.

## Why this project
Most portfolio projects show that you can break things. This one shows I can perform the task of auditors and GRC analysts, by taking a messy incident, trace it back to the specific control failures that let it happen. Then translating that into findings an executive or auditor can act on, with each recommendation tied to a real compliance control.

### Scenario Summary
National Energy, a fictional Canadian energy company (10,000+ employees, offices in Toronto, Edmonton, and Vancouver, plus a nationwide retail network), suffered a ransomeware attack that unfolded as follows:
1. Attackers exploited a vulnerbility in a third-party authentications provider, stealing valid employee credentials.
2. Using those credentials, they escalated privileges to full administrative access.
3. With admin access, they moved laterally across a flat, unsegmented network.
4. They exfiltrated sensitive data, then deployed ransomeware enterprise-wide.
5. The attack distrupted all corporate offices and halted electronic payments at retail gas stations, and went undetected until the distruption was already visible to staff.

### Skills Learned
- Cybersecurity auditing
- Technical Reporting
- ISO/IEC 27001:2022 and SOC 2 frameworks

### Tools Used
- ISO/IEC 27001:2022
- SOC 2

