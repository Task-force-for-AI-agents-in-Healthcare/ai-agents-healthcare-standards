# Appendix A: Glossary

This glossary provides definitions for terms used throughout the Healthcare AI Agents Security Verification Standard (HAAISVS). Definitions align with regulatory frameworks (FDA, EU AI Act, Health Canada, UK MHRA), healthcare industry standards, and OWASP AISVS terminology.

## A

**Adversarial Attack**: Malicious input designed to deceive AI systems, including evasion attacks (causing misclassification), poisoning attacks (corrupting training data), and prompt injection attacks (manipulating AI agent behavior).

**AI Agent**: An autonomous system that perceives its environment, makes decisions, and takes actions to achieve specific goals. In healthcare, AI agents interact with clinical systems, process patient data, and provide clinical decision support.

**AI Model Passport**: A comprehensive, machine-interpretable documentation system that tracks the complete lifecycle of an AI model including data provenance, development process, deployment parameters, and operational history.

**AISVS**: OWASP Artificial Intelligence Security Verification Standard - a framework for evaluating AI application security that HAAISVS builds upon for healthcare-specific requirements.

**Autonomous Action**: AI agent capability to execute actions without human intervention, ranging from data analysis and alert generation to direct interaction with healthcare systems and clinical workflows.

## C

**Clinical Decision Support**: AI systems that provide healthcare professionals with patient-specific assessments and evidence-based recommendations to enhance clinical decision-making.

**Clinical Function**: The primary healthcare purpose of an AI agent, categorized as diagnostic (identifying conditions), therapeutic (treatment recommendations), monitoring (patient status tracking), or administrative (workflow support).

**Clinical Workflow Integration**: The process of incorporating AI agents into existing healthcare processes while maintaining clinical efficiency, patient safety, and regulatory compliance.

**Continuous Monitoring**: Ongoing surveillance of AI agent performance, security status, and clinical effectiveness using real-time data analysis and automated alerting systems.

## D

**Data Lineage**: Complete documentation of data journey from source collection through processing, transformation, and use in AI model training and operation, including provenance, quality assessments, and bias analysis.

**Data Sensitivity**: Classification of healthcare data based on privacy requirements and regulatory protection levels, including PHI (protected health information), genomic data, behavioral health data, and anonymized clinical data.

## E

**Explainable AI (XAI)**: AI techniques that provide human-interpretable explanations for AI decision-making processes, enabling healthcare professionals to understand, validate, and trust AI agent recommendations.

**EU AI Act**: European Union legislation providing comprehensive regulation of AI systems, classifying healthcare AI applications as high-risk systems requiring enhanced oversight and compliance measures.

## F

**FDA PCCP**: Food and Drug Administration Predetermined Change Control Plan - a regulatory mechanism allowing pre-specified AI system modifications without new marketing submissions, supporting continuous improvement while maintaining safety oversight.

**FHIR (Fast Healthcare Interoperability Resources)**: HL7 standard for healthcare data exchange enabling interoperability between healthcare systems and AI agents.

## G

**GDPR**: General Data Protection Regulation - European privacy regulation affecting healthcare AI systems processing personal data, requiring consent management, data protection by design, and patient rights support.

**GMLP**: Good Machine Learning Practice - principles developed by the International Medical Device Regulators Forum (IMDRF) for safe and effective AI/ML-enabled medical devices.

## H

**HAAISVS**: Healthcare AI Agents Security Verification Standard - this standard providing security and safety verification requirements specifically for AI agents in healthcare environments.

**Healthcare AI Agent**: An autonomous AI system deployed in healthcare environments that processes clinical data, integrates with healthcare workflows, and provides clinical decision support while maintaining human oversight.

**Health Canada SGBA+**: Sex and Gender-Based Analysis Plus framework requiring assessment of healthcare interventions across diverse patient populations to prevent bias and ensure equitable outcomes.

**HIPAA**: Health Insurance Portability and Accountability Act - US healthcare privacy regulation requiring protection of patient health information and establishing security safeguards for healthcare data processing.

**Human-in-the-Loop**: System design principle ensuring human oversight and control over AI agent decisions, particularly for critical healthcare decisions affecting patient safety and care quality.

**Human Factors Engineering**: Systematic approach to optimizing human-AI interaction through usability testing, cognitive load assessment, and workflow analysis to prevent errors and support effective collaboration.

## I

**ISO/IEC 42001**: International standard for AI management systems providing framework for responsible AI development, deployment, and operation aligned with organizational governance and risk management.

**ISO 13485**: Quality management standard specifically for medical devices, applicable to AI agents classified as medical devices and requiring integration with HAAISVS requirements.

## L

**Level 1/2/3**: HAAISVS verification levels indicating requirement complexity and risk focus:
- Level 1: Foundation requirements for all healthcare AI agents
- Level 2: Advanced requirements for high-risk clinical applications  
- Level 3: Expert requirements for complex autonomous systems and research applications

## M

**Machine-Interpretable**: Documentation and data formats (JSON-LD, RDF, FHIR) that enable automated processing, compliance verification, and integration with healthcare IT systems.

**Model Drift**: Degradation of AI model performance over time due to changes in input data distribution, clinical practices, or patient populations, requiring continuous monitoring and mitigation.

**Medical Device Regulation (MDR)**: European regulation for medical devices, including AI-enabled medical devices, requiring conformity assessment and post-market surveillance.

## N

**NIST AI RMF**: National Institute of Standards and Technology AI Risk Management Framework providing governance structure (Govern, Map, Measure, Manage) for organizational AI risk management.

## O

**OWASP**: Open Web Application Security Project - organization developing security standards including AISVS for AI application security verification.

## P

**Patient-Centered Care**: Healthcare approach prioritizing patient preferences, values, and needs in clinical decision-making, which HAAISVS ensures is preserved in AI-augmented care delivery.

**PCCP**: See FDA PCCP above.

**PHI (Protected Health Information)**: Individually identifiable health information protected under HIPAA requiring special security and privacy safeguards in AI agent processing.

**Predetermined Change Control Plan**: See FDA PCCP above.

## R

**Regulatory Sandbox**: Controlled testing environment (such as UK MHRA AI Airlock) allowing healthcare AI agents to be evaluated in real-world clinical settings under regulatory oversight before full market deployment.

**Risk Assessment**: Systematic evaluation of potential harms and likelihood of occurrence, in healthcare AI focusing on patient safety, clinical workflow disruption, and data security risks.

## S

**SGBA+**: See Health Canada SGBA+ above.

**Supply Chain Security**: Protection of AI agent dependencies including pre-trained models, healthcare datasets, clinical knowledge bases, and third-party services through validation, monitoring, and integrity verification.

## T

**Three-Factor Risk Assessment**: HAAISVS methodology evaluating healthcare AI agents based on clinical function, autonomy level, and data sensitivity to determine appropriate security and oversight requirements.

**Traceability**: Ability to track and document all aspects of AI agent development, deployment, and operation, enabling regulatory compliance, clinical accountability, and incident investigation.

## U

**UK MHRA AI Airlock**: United Kingdom regulatory sandbox program allowing controlled testing of AI medical devices under regulatory oversight to generate real-world evidence for approval processes.

## V

**Verification Level**: See Level 1/2/3 above.

**Verification Requirement**: Specific, testable security or safety control that healthcare organizations, developers, or auditors can verify for compliance with HAAISVS standards.

## W

**WHO GI-AI4H**: World Health Organization Global Initiative on AI for Health providing ethical framework and governance principles for AI in healthcare, emphasizing human-centered approaches and global health equity.

## X

**XAI**: See Explainable AI above.

---

## Acronym Quick Reference

| Acronym | Full Term |
|---------|-----------|
| **AISVS** | Artificial Intelligence Security Verification Standard |
| **API** | Application Programming Interface |
| **CPOE** | Computerized Provider Order Entry |
| **DICOM** | Digital Imaging and Communications in Medicine |
| **EHR** | Electronic Health Record |
| **EMA** | European Medicines Agency |
| **FDA** | Food and Drug Administration |
| **FHIR** | Fast Healthcare Interoperability Resources |
| **GDPR** | General Data Protection Regulation |
| **GMLP** | Good Machine Learning Practice |
| **HAAISVS** | Healthcare AI Agents Security Verification Standard |
| **HIPAA** | Health Insurance Portability and Accountability Act |
| **HL7** | Health Level Seven International |
| **IEC** | International Electrotechnical Commission |
| **IMDRF** | International Medical Device Regulators Forum |
| **IRB** | Institutional Review Board |
| **ISO** | International Organization for Standardization |
| **IT** | Information Technology |
| **JSON-LD** | JavaScript Object Notation for Linked Data |
| **MDR** | Medical Device Regulation |
| **MHRA** | Medicines and Healthcare products Regulatory Agency |
| **MLOps** | Machine Learning Operations |
| **NHS** | National Health Service |
| **NIST** | National Institute of Standards and Technology |
| **OWASP** | Open Web Application Security Project |
| **PCCP** | Predetermined Change Control Plan |
| **PHI** | Protected Health Information |
| **PII** | Personally Identifiable Information |
| **RDF** | Resource Description Framework |
| **SGBA+** | Sex and Gender-Based Analysis Plus |
| **SIEM** | Security Information and Event Management |
| **SOC** | Security Operations Center / Service Organization Control |
| **WHO** | World Health Organization |
| **XAI** | Explainable Artificial Intelligence |

---

*This glossary is maintained by the Task Force for AI Agents in Healthcare and updated regularly to reflect evolving healthcare AI terminology and regulatory requirements.*
