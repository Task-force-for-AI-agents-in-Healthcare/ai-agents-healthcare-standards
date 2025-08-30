# Using the HAARF

The Healthcare AI Agents Security Verification Standard (HAARF) defines security and safety requirements for autonomous AI agents in healthcare environments, focusing on aspects within the control of healthcare organizations, AI developers, and clinical implementation teams.

The HAARF is intended for anyone developing, deploying, or evaluating the security and safety of healthcare AI agents, including clinical teams, AI developers, healthcare security professionals, regulatory affairs specialists, and compliance auditors. This chapter introduces the structure and use of HAARF, including its verification levels and healthcare-specific implementation guidance.

## Healthcare AI Agent Security Verification Levels

The HAARF defines three ascending levels of security verification, each tailored to the risk profile and clinical impact of AI agents in healthcare environments. Each level adds depth and complexity, enabling healthcare organizations to tailor their security posture to match patient safety requirements and regulatory obligations.

Healthcare organizations should begin at Level 1 for all clinical AI agents and progressively adopt higher levels based on clinical risk, patient population, and regulatory requirements.

### Definition of the Levels

Each requirement in HAARF v1.0 is assigned to one of the following levels:

#### Level 1: Foundation Healthcare Security (All Clinical AI Agents)
**Target**: Every AI agent deployed in clinical or patient-facing healthcare environments  
**Regulatory Basis**: FDA Class II medical device equivalent, EU AI Act high-risk systems

Level 1 includes the most critical healthcare-specific security requirements that prevent common attacks and ensure basic patient safety. These controls focus on:
- **Patient Safety Fundamentals**: Core requirements that prevent patient harm
- **Clinical Workflow Protection**: Basic integration security for healthcare systems  
- **Healthcare Data Privacy**: Essential HIPAA/GDPR compliance for medical AI
- **Human Oversight**: Mandatory human-in-the-loop requirements for clinical decisions

*All healthcare AI agents must achieve Level 1 compliance before clinical deployment.*

#### Level 2: Advanced Healthcare Security (High-Risk Clinical Applications)
**Target**: AI agents handling critical patient decisions, life-supporting systems, diagnostic AI  
**Regulatory Basis**: FDA Class III medical device equivalent, EU AI Act enhanced oversight

Level 2 addresses advanced attacks and layered defenses for high-risk healthcare applications. These requirements focus on:
- **Advanced Threat Protection**: Healthcare-specific adversarial attack prevention
- **Enhanced Traceability**: Complete AI Model Passport with clinical audit trails
- **Regulatory Compliance**: Full PCCP implementation and continuous monitoring  
- **Clinical Decision Validation**: Advanced human factors and clinical oversight

*Required for AI agents involved in diagnosis, treatment recommendations, or critical care.*

#### Level 3: Expert Healthcare Security (Research & Complex Autonomous Systems)
**Target**: Multi-agent systems, research applications, autonomous surgical systems  
**Regulatory Basis**: FDA breakthrough device pathway, EU AI Act conformity assessment

Level 3 includes controls for the most sophisticated healthcare AI deployments. These requirements focus on:
- **Research-Grade Security**: Advanced security for experimental AI applications
- **Multi-Agent Coordination**: Security for AI agent swarms and collaborative systems
- **Advanced Analytics**: Predictive security monitoring and threat intelligence
- **Regulatory Innovation**: Support for regulatory sandbox and breakthrough device pathways

*Appropriate for cutting-edge AI research, complex autonomous systems, and novel healthcare applications.*

### Healthcare-Specific Risk Classification

HAARF risk levels align with established healthcare risk classification frameworks:

#### Clinical Risk Factors
- **Patient Population**: Pediatric, elderly, critical care, emergency medicine (higher risk)
- **Clinical Function**: Diagnostic, therapeutic, monitoring, administrative (diagnostic/therapeutic = higher risk)  
- **Decision Autonomy**: Alert/recommend, decision support, autonomous action (autonomous = higher risk)
- **Data Sensitivity**: Administrative, clinical, genomic, behavioral health (genomic/behavioral = higher risk)

#### Regulatory Risk Mapping
| HAARF Level | FDA Classification | EU AI Act Category | Health Canada Class |
|:-------------:|:-----------------:|:-----------------:|:-------------------:|
| **Level 1**   | Class II Medical Device | High-Risk AI System | Class II/III |
| **Level 2**   | Class III Medical Device | High-Risk + Enhanced | Class III/IV |
| **Level 3**   | Breakthrough Device | Conformity Assessment | Class IV Research |

### Role Designations (H/D/V/C)

Each HAARF requirement is marked according to the primary healthcare stakeholder audience:

* **H** – Healthcare organization/clinical team-focused requirements
* **D** – AI developer/technical team-focused requirements  
* **V** – Verifier/auditor/compliance-focused requirements
* **C** – Clinical/medical professional-focused requirements
* **H/D/V/C** – Requirements relevant to multiple stakeholders

### Implementation Pathways by Healthcare Setting

#### Hospital & Health System Implementation
**Recommended Approach**: Start with Level 1 across all AI agents, advance to Level 2 for critical care applications
```
Phase 1: Level 1 compliance for all clinical AI agents (6 months)
Phase 2: Level 2 for diagnostic and therapeutic AI (12 months)  
Phase 3: Level 3 for research and autonomous systems (24 months)
```

#### Medical Device Manufacturers
**Recommended Approach**: Integrate HAARF into medical device quality management system
```
Development: Level 1 requirements in design controls
Validation: Level 2 verification and validation testing
Submission: Level 2/3 for regulatory submissions (FDA 510k, EU CE marking)
```

#### Healthcare AI Startups & Vendors  
**Recommended Approach**: Build HAARF compliance into product development lifecycle
```
MVP: Level 1 core security and safety requirements
Clinical Pilots: Level 2 enhanced security and traceability
Commercial Launch: Level 2 regulatory compliance + Level 3 for differentiation
```

#### Regulatory Affairs & Compliance Teams
**Recommended Approach**: Use HAARF as regulatory submission framework
```
Gap Analysis: Assess current AI agents against HAARF requirements
Remediation: Address Level 1 gaps before clinical deployment
Submission: Use HAARF verification as evidence for regulatory compliance
```

### Regulatory Submission Integration

HAARF verification requirements directly support regulatory submissions:

- **FDA 510(k)**: HAARF Level 2 provides predicate device equivalency evidence
- **FDA De Novo**: HAARF Level 3 supports novel device classification requests  
- **EU CE Marking**: HAARF aligns with AI Act conformity assessment requirements
- **Health Canada MDPD**: HAARF verification supports SGBA+ bias mitigation evidence
- **UK MHRA AI Airlock**: HAARF provides structured evidence for sandbox applications

Healthcare organizations and AI developers can use HAARF compliance documentation directly in regulatory submissions, reducing time-to-market and improving approval success rates.

---

**HAARF provides healthcare-specific verification requirements that ensure AI agents are not only technically secure but also clinically safe, regulatory compliant, and aligned with the highest standards of patient care.**
