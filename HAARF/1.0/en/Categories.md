# HAARF v1.0 Categories Overview

The **Healthcare AI Agents Regulatory Framework (HAARF)** v1.0 defines regulatory compliance and safety requirements across **eight comprehensive categories**, each addressing critical aspects of healthcare AI agent deployment. These categories reflect the unique requirements of healthcare environments, align with global regulatory frameworks, and incorporate insights from the Healthcare AI Agents Working Group meetings with FDA industry committee stakeholders.

**Built upon OWASP AISVS Foundation**: HAARF is adapted from the excellent [OWASP Artificial Intelligence Security Verification Standard (AISVS)](https://github.com/OWASP/AISVS) framework, specialized for healthcare regulatory compliance.

## License

This work is licensed under the **[Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/)**.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

## Category Structure

Each category follows a consistent structure designed for healthcare compliance and regulatory alignment:

- **Control Objective**: High-level security goal aligned with healthcare standards
- **Subcategories**: Specific functional areas within each category
- **Verification Requirements**: Detailed, testable requirements with healthcare context
- **Level Assignment**: Risk-based categorization (1, 2, 3)
- **Role Designation**: Target stakeholder (H/D/V/C)
- **Healthcare Integration**: Clinical workflow and regulatory compliance focus

## C1: Unified Risk & Lifecycle Assessment

**Total Requirements**: 24 verification requirements  
**Regulatory Basis**: FDA PCCP, EU AI Act, Health Canada SGBA+, UK MHRA  
**Clinical Focus**: Patient safety risk management and regulatory compliance

### Subcategories
- **C1.1** Healthcare Risk Classification & Assessment (6 requirements)
- **C1.2** FDA-Style Predetermined Change Control Plans (6 requirements)  
- **C1.3** Continuous Clinical Performance Monitoring (6 requirements)
- **C1.4** Regulatory Sandbox & Real-World Evidence (5 requirements)
- **C1.5** International Regulatory Harmonization (4 requirements)
- **C1.6** Clinical Risk Management Integration (5 requirements)

### Key Healthcare Innovations
- Three-factor risk assessment (clinical function, autonomy, data sensitivity)
- Healthcare-specific PCCP implementation for FDA compliance
- Clinical performance monitoring with Health Canada SGBA+ requirements
- Integration with healthcare risk management and patient safety systems

## C2: AI Model Passport & Traceability

**Total Requirements**: 34 verification requirements  
**Regulatory Basis**: All jurisdictions - universal traceability requirement  
**Clinical Focus**: Complete lifecycle documentation and clinical accountability

### Subcategories  
- **C2.1** Data Lineage & Health Canada SGBA+ Compliance (6 requirements)
- **C2.2** Model Development & Versioning Traceability (6 requirements)
- **C2.3** Explainable AI (XAI) & Decision Transparency (6 requirements)
- **C2.4** Clinical Decision Audit Trails (6 requirements)
- **C2.5** Regulatory Compliance Documentation (5 requirements)
- **C2.6** Machine-Interpretable Documentation (5 requirements)
- **C2.7** Healthcare Supply Chain Transparency (4 requirements)

### Key Healthcare Innovations
- Healthcare-specific data lineage with bias assessment
- Clinical explainable AI tailored for healthcare professionals
- Integration with EHR and clinical documentation systems
- Automated regulatory compliance reporting for multiple jurisdictions

## C3: Proactive Cybersecurity Framework

**Total Requirements**: 35 verification requirements  
**Regulatory Basis**: NIST, OWASP AISVS, healthcare cybersecurity standards  
**Clinical Focus**: Healthcare data protection and clinical system security

### Subcategories
- **C3.1** Healthcare-Specific Adversarial Robustness (6 requirements)
- **C3.2** Healthcare AI Supply Chain Security (6 requirements)
- **C3.3** Real-Time Healthcare Threat Monitoring (6 requirements)
- **C3.4** OWASP AISVS Healthcare Alignment (5 requirements)
- **C3.5** Healthcare Data Protection & Privacy Security (6 requirements)
- **C3.6** Clinical Incident Response & Recovery (6 requirements)
- **C3.7** Healthcare Penetration Testing & Red Team Exercises (5 requirements)

### Key Healthcare Innovations
- Healthcare-specific adversarial attack protection (medical imaging, clinical data)
- Integration with healthcare security operations and clinical incident response
- HIPAA/GDPR-compliant data protection with clinical workflow integration
- Healthcare-specific penetration testing including clinical scenario simulation

## C4: Human-in-the-Loop Oversight

**Total Requirements**: 38 verification requirements  
**Regulatory Basis**: WHO GI-AI4H, clinical professional standards  
**Clinical Focus**: Healthcare professional empowerment and patient-centered care

### Subcategories
- **C4.1** Clinical Accountability & Responsibility Frameworks (6 requirements)
- **C4.2** Clinical Decision Validation & Override Capabilities (6 requirements)
- **C4.3** Healthcare Human Factors Engineering & Usability (6 requirements)
- **C4.4** Clinical Competency & Training Requirements (6 requirements)
- **C4.5** Patient Communication & Informed Consent (6 requirements)
- **C4.6** Clinical Workflow Integration & Change Management (6 requirements)
- **C4.7** Quality Improvement & Clinical Outcome Monitoring (6 requirements)
- **C4.8** Ethics & Patient-Centered Care Preservation (6 requirements)

### Key Healthcare Innovations
- Clinical accountability frameworks preserving healthcare professional responsibility
- Human factors engineering following medical device usability standards
- Patient communication and consent frameworks for AI transparency
- Integration with healthcare quality improvement and clinical governance

## C5: Agent Registration & Identity Management

**Total Requirements**: 30 verification requirements  
**Regulatory Basis**: Network security, healthcare asset management, FDA device registration  
**Clinical Focus**: Agent visibility, network security, and operational control

### Subcategories
- **C5.1** Healthcare Agent Registration & Cataloging (6 requirements)
- **C5.2** Agent Identity Verification & Authentication (6 requirements)
- **C5.3** Agent Lifecycle Registration Management (6 requirements)
- **C5.4** Cross-Platform Agent Interoperability (5 requirements)
- **C5.5** Agent Behavioral Monitoring & Anomaly Detection (5 requirements)
- **C5.6** Regulatory Compliance Integration (5 requirements)

### Key Healthcare Innovations
- Healthcare-specific agent ID systems integrated with medical device management
- Cross-platform agent identity supporting HL7 FHIR and healthcare interoperability
- Behavioral monitoring tailored for clinical environments and workflow protection
- Integration with healthcare security operations centers and clinical incident response

## C6: Agent Autonomy Levels & Governance

**Total Requirements**: 35 verification requirements  
**Regulatory Basis**: Progressive autonomy management, clinical decision authority, patient safety  
**Clinical Focus**: Safe autonomy progression and human-agent authority boundaries

### Subcategories
- **C6.1** Autonomy Level Classification & Assessment (6 requirements)
- **C6.2** Progressive Autonomy Implementation (6 requirements)
- **C6.3** Human-Agent Authority Boundaries (6 requirements)
- **C6.4** Autonomous Agent Containment & Safety Limits (6 requirements)
- **C6.5** Multi-Agent Coordination & Governance (5 requirements)
- **C6.6** Autonomy Performance Monitoring & Optimization (5 requirements)
- **C6.7** Emergency Override & Manual Control (5 requirements)

### Key Healthcare Innovations
- Standardized autonomy level classification from co-pilot to full autonomy
- Progressive autonomy with mandatory clinical validation gates
- Healthcare-specific authority boundaries aligned with clinical scope of practice
- Emergency override capabilities preserving clinical decision-making authority

## C7: Bias Mitigation & Population Equity

**Total Requirements**: 35 verification requirements  
**Regulatory Basis**: Health equity, non-discrimination, vulnerable population protection  
**Clinical Focus**: Equitable AI performance across diverse patient populations

### Subcategories
- **C7.1** Training Data Representativeness & Demographic Parity (6 requirements)
- **C7.2** Algorithmic Bias Detection & Assessment (6 requirements)
- **C7.3** Bias Mitigation & Fairness Enhancement (6 requirements)
- **C7.4** Vulnerable Population Protection (6 requirements)
- **C7.5** Global Health Equity & Resource-Limited Settings (5 requirements)
- **C7.6** Continuous Equity Monitoring & Improvement (6 requirements)
- **C7.7** Regulatory Compliance & Equity Reporting (5 requirements)

### Key Healthcare Innovations
- Comprehensive demographic representation requirements beyond SGBA+
- Intersectional bias analysis for multiple demographic characteristics
- Vulnerable population protection with enhanced clinical safeguards
- Global health equity considerations for resource-limited healthcare settings

## C8: Tool Use & Integration Security ⭐ *FDA Priority Enhancement*

**Total Requirements**: 42 verification requirements  
**Regulatory Basis**: FDA medical device integration, tool combination regulatory pathways  
**Clinical Focus**: Safe and compliant use of medical tools, APIs, and healthcare systems by AI agents

### Subcategories
- **C8.1** Tool Authorization & Access Control (6 requirements)
- **C8.2** Tool Selection & Clinical Appropriateness (6 requirements)
- **C8.3** Medical Device Integration & Interoperability (6 requirements)
- **C8.4** API Security & Healthcare System Access (6 requirements)
- **C8.5** Cascading Failure Prevention & System Resilience (5 requirements)
- **C8.6** Tool Performance Monitoring & Optimization (5 requirements)
- **C8.7** Regulatory Compliance for Tool-Enabled Agents (8 requirements)

### Key Healthcare Innovations
- FDA-compliant medical device integration without altering device classification
- Role-based tool access controls with clinical appropriateness validation
- Evidence-based tool selection with contraindication checking and safety validation
- Circuit breaker patterns and isolation mechanisms to prevent cascading failures
- Comprehensive regulatory pathway analysis for tool combination FDA submissions
- Quality system integration for manufacturing controls of tool-enabled agents

### FDA Priority Significance
C8 addresses the fundamental capability that differentiates AI agents from traditional AI/ML medical devices: **the ability to autonomously select, access, and use multiple healthcare tools and systems**. This represents the most critical regulatory gap for tool-enabled healthcare AI agents and provides clear guidance for FDA submission pathways including 510(k), PMA, and breakthrough device considerations.

## Cross-Category Integration

HAARF categories are designed for integrated implementation:

### Regulatory Compliance Integration
- **C1 + C2**: Risk assessment with complete traceability for regulatory submissions
- **C2 + C3**: Secure documentation and audit trails supporting compliance verification
- **C1 + C4**: Human oversight integrated with risk management and clinical governance

### Clinical Workflow Integration  
- **C3 + C4**: Secure human-AI collaboration with clinical usability optimization
- **C2 + C4**: Explainable AI supporting clinical decision validation and override
- **C1 + C3**: Risk-based security controls with clinical safety integration

### Healthcare Organization Implementation
- **All Categories**: Comprehensive framework supporting healthcare organization AI governance
- **Scalable Implementation**: Level-based progression from foundational to advanced requirements
- **Role-Based Deployment**: Clear stakeholder responsibilities across healthcare teams

## Level Distribution Summary

| Level | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | Total |
|:-----:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:-----:|
| **1** | 9 | 8 | 12 | 14 | 12 | 8 | 10 | 12 | 85 |
| **2** | 13 | 20 | 18 | 18 | 15 | 20 | 20 | 20 | 144 |
| **3** | 8 | 6 | 5 | 6 | 3 | 7 | 5 | 10 | 50 |
| **Total** | **30** | **34** | **35** | **38** | **30** | **35** | **35** | **42** | **279** |

## Role Distribution Summary

| Role | Description | Est. Requirements | Primary Stakeholders |
|:----:|------------|:----------------:|---------------------|
| **H** | Healthcare Organization | 85 | Hospitals, clinics, health systems |
| **D** | Developer/Technical | 75 | AI developers, MLOps engineers, technical teams |
| **V** | Verifier/Auditor | 70 | Compliance teams, auditors, regulatory affairs |
| **C** | Clinical Professional | 65 | Physicians, nurses, clinical specialists |

*Note: Many requirements are multi-role (H/D, D/V, H/C, etc.), so role counts reflect estimated primary responsibility distribution across the expanded 279 requirements.*

## Working Group Integration

The HAARF v1.0 framework incorporates key insights from the **Healthcare AI Agents Working Group** meetings with FDA industry committee stakeholders:

### **Pete Jarvis's Five Focus Areas** (Fully Integrated)
✅ **Clinical Risk Alignment** → C1: Unified Risk & Lifecycle Assessment  
✅ **Autonomy & Oversight Gradient** → C6: Agent Autonomy Levels & Governance  
✅ **Lifecycle Artifact Traceability** → C2: AI Model Passport & Traceability  
✅ **Tier-based Regulatory Pathways** → C1 + C5 + C6 (Risk-based approaches)  
✅ **Shared Responsibility & Governance** → C4 + C6 + C7 (Human oversight & governance)

### **Community-Identified Priorities**
✅ **Agent Registration & Identity** (Jim Schwoebel) → C5: Agent Registration & Identity Management  
✅ **Population Equity & Bias** (Donna Russell) → C7: Bias Mitigation & Population Equity  
✅ **Multi-jurisdictional Compliance** (Phil Englert) → Integrated across all categories  
✅ **Security & Offensive Testing** (Kyle Quest, Pete Jarvis) → C3: Proactive Cybersecurity Framework

### **FDA Priority Enhancement**
⭐ **Tool Use & Integration Security** → C8: Tool Use & Integration Security *(Added based on direct FDA feedback identifying the critical regulatory gap for tool-enabled healthcare AI agents - the fundamental capability that differentiates AI agents from traditional AI/ML medical devices)*

---

**HAARF v1.0 provides the world's most comprehensive healthcare AI agent security verification standard with 279 specific requirements across eight categories, ensuring clinical safety, regulatory compliance, population equity, and human-centered care preservation for all healthcare environments.**
