# HAAISVS Regulatory Framework Mappings

This directory contains mappings between HAAISVS verification requirements and various healthcare regulatory frameworks, security standards, and compliance requirements. These mappings support regulatory submissions, compliance verification, and gap analysis across multiple jurisdictions.

## Available Mappings

### Regulatory Authority Mappings
- **[fda-mapping.json](fda-mapping.json)** - FDA medical device regulations, Digital Health guidance, and PCCP requirements
- **[eu-ai-act-mapping.json](eu-ai-act-mapping.json)** - EU AI Act high-risk system requirements and MDR/IVDR integration
- **[health-canada-mapping.json](health-canada-mapping.json)** - Health Canada ML-enabled medical device guidance and SGBA+ requirements
- **[uk-mhra-mapping.json](uk-mhra-mapping.json)** - UK MHRA AI regulation and AI Airlock sandbox requirements

### International Standards Mappings  
- **[nist-ai-rmf-mapping.json](nist-ai-rmf-mapping.json)** - NIST AI Risk Management Framework alignment
- **[iso-42001-mapping.json](iso-42001-mapping.json)** - ISO/IEC 42001 AI management system standards
- **[who-gi-ai4h-mapping.json](who-gi-ai4h-mapping.json)** - WHO Global Initiative on AI for Health principles
- **[imdrf-gmlp-mapping.json](imdrf-gmlp-mapping.json)** - IMDRF Good Machine Learning Practice principles

### Healthcare Industry Standards
- **[iso-13485-mapping.json](iso-13485-mapping.json)** - ISO 13485 medical device quality management
- **[hipaa-mapping.json](hipaa-mapping.json)** - HIPAA privacy and security requirements for healthcare AI
- **[gdpr-mapping.json](gdpr-mapping.json)** - GDPR data protection requirements for healthcare AI
- **[hl7-fhir-mapping.json](hl7-fhir-mapping.json)** - HL7 FHIR healthcare interoperability standards

### Security Standards Mappings
- **[owasp-aisvs-mapping.json](owasp-aisvs-mapping.json)** - OWASP AISVS security verification standard alignment
- **[nist-cybersecurity-mapping.json](nist-cybersecurity-mapping.json)** - NIST Cybersecurity Framework for healthcare
- **[iso-27001-mapping.json](iso-27001-mapping.json)** - ISO/IEC 27001 information security management

## Mapping Format

Each mapping file uses standardized JSON format for automated processing:

```json
{
  "mapping_info": {
    "haaisvs_version": "1.0",
    "target_framework": "Framework Name",
    "target_version": "Framework Version",
    "mapping_date": "2025-01-10",
    "mapping_status": "complete|partial|in_progress"
  },
  "mappings": [
    {
      "haaisvs_requirement": "1.1.1",
      "target_requirements": ["Target-Req-1", "Target-Req-2"],
      "alignment_type": "direct|partial|gap",
      "notes": "Explanation of alignment or gaps",
      "compliance_evidence": "Required documentation or testing"
    }
  ],
  "coverage_analysis": {
    "total_haaisvs_requirements": 137,
    "mapped_requirements": 120,
    "direct_alignment": 85,
    "partial_alignment": 35,
    "gaps_identified": 17
  }
}
```

## Alignment Types

### Direct Alignment
HAAISVS requirement directly corresponds to target framework requirement with equivalent scope and intent.

### Partial Alignment  
HAAISVS requirement partially addresses target framework requirement but may require additional controls or documentation.

### Gap Identified
Target framework requirement not fully addressed by current HAAISVS requirements, indicating potential enhancement areas.

## Usage Instructions

### For Regulatory Submissions
1. Identify target regulatory framework (FDA, EU AI Act, Health Canada, UK MHRA)
2. Use corresponding mapping file to identify required HAAISVS verification levels
3. Generate compliance evidence documentation using mapping guidance
4. Include mapping analysis in regulatory submission documentation

### For Compliance Verification
1. Select relevant mapping files for applicable regulatory requirements
2. Conduct gap analysis identifying requirements needing additional controls
3. Implement necessary HAAISVS verification requirements
4. Document compliance evidence according to mapping specifications

### For Multi-Jurisdictional Deployment
1. Combine multiple mapping files for target markets
2. Identify highest level requirements across all jurisdictions  
3. Implement comprehensive HAAISVS compliance covering all regulatory requirements
4. Maintain separate compliance documentation for each jurisdiction

## Mapping Maintenance

Mappings are updated regularly to reflect:
- Regulatory framework changes and updates
- New healthcare AI guidance documents
- Stakeholder feedback and implementation experience
- International harmonization developments

### Update Schedule
- **Quarterly Reviews**: Regulatory guidance updates and framework changes
- **Annual Updates**: Comprehensive mapping validation and enhancement
- **Event-Driven Updates**: Major regulatory announcements or framework releases

### Contribution Guidelines
Organizations and experts can contribute to mapping accuracy by:
1. Submitting mapping corrections or enhancements via GitHub issues
2. Providing implementation experience and compliance evidence examples
3. Sharing regulatory feedback and submission outcomes
4. Participating in mapping validation reviews

## Cross-Reference Integration

Mappings support automated compliance tools through:
- **JSON Schema Validation**: Ensuring mapping file consistency and accuracy
- **API Integration**: Enabling automated compliance checking and reporting
- **Database Integration**: Supporting compliance management systems
- **Documentation Generation**: Automating regulatory submission documentation

---

*Regulatory framework mappings are maintained by the Task Force for AI Agents in Healthcare with input from regulatory affairs professionals, compliance experts, and healthcare organizations worldwide.*
