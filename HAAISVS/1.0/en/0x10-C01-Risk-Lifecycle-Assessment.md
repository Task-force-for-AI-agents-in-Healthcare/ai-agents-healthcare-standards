# C1 Unified Risk & Lifecycle Assessment

## Control Objective

Healthcare AI agents must undergo comprehensive risk assessment and continuous lifecycle management that aligns with FDA Total Product Lifecycle approach, EU AI Act high-risk classification, and Health Canada SGBA+ requirements. This ensures that AI agents maintain safety, effectiveness, and regulatory compliance throughout their operational lifespan while adapting to evolving clinical environments and patient populations.

---

## C1.1 Healthcare Risk Classification & Assessment

Implement three-factor risk assessment (clinical function, autonomy level, data sensitivity) aligned with medical device regulatory frameworks.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.1.1** | **Verify that** all healthcare AI agents undergo mandatory three-factor risk assessment evaluating clinical function (diagnostic, therapeutic, monitoring, administrative), autonomy level (alert, decision support, autonomous action), and data sensitivity (PHI, genomic, behavioral health) before clinical deployment. | 1 | H/V |
| **1.1.2** | **Verify that** AI agents handling diagnostic or therapeutic functions are automatically classified as high-risk regardless of other factors, requiring enhanced verification and clinical oversight. | 1 | H/V |
| **1.1.3** | **Verify that** risk assessment outcomes map to established medical device classification frameworks (FDA Class I/II/III, EU MDR risk classes, Health Canada Class I-IV). | 1 | V |
| **1.1.4** | **Verify that** patient population risk factors (pediatric, elderly, critical care, emergency medicine) are explicitly evaluated and documented in risk assessment outcomes. | 2 | H/C |
| **1.1.5** | **Verify that** risk assessments include healthcare-specific threat modeling covering clinical workflow disruption, patient safety incidents, and medical data breach scenarios. | 2 | H/V |
| **1.1.6** | **Verify that** risk classification decisions undergo clinical review by qualified healthcare professionals with AI competency. | 3 | C |

---

## C1.2 FDA-Style Predetermined Change Control Plans (PCCP)

Implement change control plans that pre-specify allowable AI agent modifications without requiring new regulatory submissions.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.2.1** | **Verify that** all high-risk healthcare AI agents implement FDA-style Predetermined Change Control Plans (PCCP) specifying types of modifications, validation processes, and performance acceptance criteria before initial clinical deployment. | 1 | D/V |
| **1.2.2** | **Verify that** PCCP specifications include clinical performance metrics, patient safety monitoring parameters, and healthcare workflow integration requirements that must be maintained across agent updates. | 1 | H/D |
| **1.2.3** | **Verify that** all AI agent modifications are evaluated against PCCP criteria before implementation, with deviations requiring new risk assessment and potential regulatory submission. | 2 | D/V |
| **1.2.4** | **Verify that** PCCP implementation includes automated testing protocols that validate clinical safety, performance maintenance, and regulatory compliance for each agent modification. | 2 | D/V |
| **1.2.5** | **Verify that** PCCP documentation undergoes clinical review and regulatory affairs validation before submission to relevant healthcare authorities (FDA, EMA, Health Canada). | 3 | V |
| **1.2.6** | **Verify that** PCCP effectiveness is continuously monitored with metrics tracked for modification success rates, clinical performance stability, and regulatory compliance maintenance. | 3 | H/V |

---

## C1.3 Continuous Clinical Performance Monitoring

Implement real-time monitoring systems that detect performance degradation, model drift, and clinical safety issues.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.3.1** | **Verify that** healthcare AI agents implement continuous monitoring systems that track clinical performance metrics, patient safety indicators, and healthcare workflow integration effectiveness. | 1 | H/D |
| **1.3.2** | **Verify that** performance monitoring includes automated detection of model drift, accuracy degradation, and bias emergence across different patient populations and clinical scenarios. | 1 | D/V |
| **1.3.3** | **Verify that** monitoring systems maintain statistical significance testing and alert healthcare teams when performance degrades below clinically acceptable thresholds. | 2 | H/D |
| **1.3.4** | **Verify that** clinical performance data is continuously analyzed for Health Canada SGBA+ compliance, ensuring maintained performance across diverse patient demographics. | 2 | H/V |
| **1.3.5** | **Verify that** monitoring systems integrate with healthcare quality improvement processes and clinical incident reporting systems. | 2 | H/C |
| **1.3.6** | **Verify that** advanced monitoring includes predictive analytics that identify potential performance issues before they impact patient care. | 3 | D/V |

---

## C1.4 Regulatory Sandbox & Real-World Evidence

Leverage regulatory sandbox approaches for controlled testing and evidence generation in clinical environments.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.4.1** | **Verify that** healthcare AI agents undergo controlled testing in regulatory sandbox environments (UK MHRA AI Airlock, FDA Pre-Cert pilot) when available for the intended clinical use case. | 2 | H/V |
| **1.4.2** | **Verify that** real-world evidence collection protocols are established for healthcare AI agents, capturing clinical effectiveness, safety outcomes, and healthcare workflow impact data. | 2 | H/C |
| **1.4.3** | **Verify that** sandbox testing includes diverse patient populations and clinical scenarios representative of intended deployment environments. | 2 | H/C |
| **1.4.4** | **Verify that** evidence generation protocols align with regulatory authority requirements for post-market surveillance and clinical effectiveness demonstration. | 3 | V |
| **1.4.5** | **Verify that** sandbox results and real-world evidence are systematically integrated into continuous improvement processes and regulatory submissions. | 3 | H/V |

---

## C1.5 International Regulatory Harmonization

Ensure compliance with multiple international regulatory frameworks for global healthcare AI deployment.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.5.1** | **Verify that** healthcare AI agents meet harmonized requirements across major regulatory jurisdictions (FDA, EU AI Act, Health Canada, UK MHRA) for intended markets. | 2 | V |
| **1.5.2** | **Verify that** regulatory compliance documentation supports mutual recognition and reciprocity agreements between healthcare authorities. | 3 | V |
| **1.5.3** | **Verify that** AI agent design and validation processes incorporate IMDRF Good Machine Learning Practice (GMLP) principles for international harmonization. | 3 | D/V |
| **1.5.4** | **Verify that** compliance frameworks align with WHO GI-AI4H principles for global health equity and accessible healthcare AI deployment. | 3 | H/V |

---

## C1.6 Clinical Risk Management Integration

Integrate AI agent risk management with existing healthcare risk management and patient safety systems.

| # | Description | Level | Role |
|:--------:|---------------------------------------------------------------------------------------------------------------------|:---:|:---:|
| **1.6.1** | **Verify that** AI agent risk management integrates with organizational healthcare risk management systems and clinical governance structures. | 1 | H |
| **1.6.2** | **Verify that** AI-related incidents are captured in healthcare incident reporting systems with appropriate root cause analysis and corrective action processes. | 1 | H/C |
| **1.6.3** | **Verify that** clinical risk management includes specific protocols for AI agent failure modes, backup procedures, and manual override capabilities. | 2 | H/C |
| **1.6.4** | **Verify that** risk management processes include patient safety officers and clinical leadership in AI agent oversight and incident response. | 2 | H/C |
| **1.6.5** | **Verify that** advanced risk management incorporates predictive risk analytics and proactive incident prevention for AI agent deployments. | 3 | H |

---

**Control Category C1 ensures that healthcare AI agents undergo comprehensive risk assessment and lifecycle management aligned with global regulatory requirements, maintaining clinical safety and regulatory compliance throughout their operational deployment.**
