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

### Key Findings
| # | Finding | Severity | Mapped Controls |
|--------------------|-------------------------|----------------------|-------------------------|
| A | Third-party risk management | High | ISO 27001 A 5.19 · SOC 2 CC9.2 |
| B | Identity & privileged access management | Critical | ISO 27001 A 8.2 · SOC 2 CC6.3 |
| C | Authentication control deficiency | High | ISO 27001 A 5.15, A 8.5 · SOC 2 CC6.1, CC6.2 |
| D | Network Segmentation & lateral movement | Critical | ISO 27001 A 8.20, A 8.22 · SOC 2 CC6.1 |
| E | Security monitoring & incident detection | Critical | ISO 27001 A 5.24 · SOC 2 CC7.2-CC7.4 |
| F | Endpoint security controls | Critical | ISO 27001 A 8.7 · SOC 2 CC6.8 |

**Overall audit opinion:** the control environment would not provide reasonable assurance to an ISO/IEC 27001:2022 or SOC 2 Type II assessor that logical access, system operators, or supplier risk are effecitvley managed.

### Recommendations
| Priority | Timeline | Recommendation |
|--------------------|-------------------------|----------------------|
| Critical | 0-30 days | Deploy enterprise EDR with behavioural detection and auto-isolation |
| Critical | 0-30 days | Overhaul IAM/PAM: RBAC, MFA, just-in-time admin access, quarterly access reviews |
| High | 30-90 days | Redesign network architecture: segmentation, VLANs, IDS/IPS, Zero Trust principles |
| High | 30-90 days | Formalize third-party risk management program with contractual security requirements |
| High | 30-90 days | Stregthen backup/recovery: Immutable offline backups, tested RTOs/RPOs |
| High | 30-90 days | Stand up formal SOC/incident response capabiltiy with SIEM and defined escalation paths |
| Medium | 90-180 days | Build a security awareness and communication program |

Each recommendation in the full report includes the specific control objective, business risk, expected audit evidence, and framework citations.

### Skills Demonstrated
- **Cybersecurity auditing:** control gap analysis against ISO/IEC 27001:2022 Annex A and SOC 2 Trust Services Criteria
- **Incident analysis:** reconstructing and mapping an attack lifestyle (inital access → privilege escalation → lateral movement → exfiltration → impact)
- **Risk assessment:** rating findings by likelihood/impact and assigning remediation priority
- **Technical report writing:** producing audit-ready documentation for executive and compliance audiences
- **Framework literacy:** translating technical findings into specific, citable control references

### Frameworks Referenced
- ISO/IEC 27001:2022 (Annex A controls)
- SOC 2 (Security & Availability Trust Services Criteria)

*This is a fictional case study created for portfolio purposes. National Energy, its personnel, and the described incident are not real.*
