# HAARF v1.0 Regulatory Framework Mappings

This directory contains comprehensive mappings between HAARF v1.0 and major global regulatory frameworks for healthcare AI agents.

## 📋 Available Mappings

| Framework | File | Coverage | Status |
|-----------|------|----------|--------|
| **FDA Digital Health** | `fda-mapping.json` | 234/279 (84%) | ✅ Complete |
| **EU AI Act** | `eu-ai-act-mapping.json` | 198/279 (71%) | ✅ Complete |
| **Health Canada SGBA+** | `health-canada-mapping.json` | 187/279 (67%) | ✅ Complete |
| **UK MHRA** | `uk-mhra-mapping.json` | 167/279 (60%) | ✅ Complete |
| **NIST AI RMF** | `nist-ai-rmf-mapping.json` | 245/279 (88%) | ✅ Complete |
| **OWASP AISVS** | `owasp-aisvs-mapping.json` | 156/279 (56%) | ✅ Complete |
| **WHO GI-AI4H** | `who-gi-ai4h-mapping.json` | 134/279 (48%) | ✅ Complete |
| **ISO/IEC 42001** | `iso-iec-42001-mapping.json` | 198/279 (71%) | ✅ Complete |
| **IMDRF GMLP** | `imdrf-gmlp-mapping.json` | 201/279 (72%) | ✅ Complete |

**Total HAARF Requirements**: 279 across 8 categories  
**Average Coverage**: 69% across all frameworks

## 🎯 FDA Priority Enhancement

Mappings reflect FDA's highest priority feedback leading to **C8: Tool Use & Integration Security**:

> *"The enhanced HAARF framework with C8 (Tool Use) represents the most comprehensive guidance available for medical device companies developing AI agents."*

## 📊 Alignment Types

- **Direct**: HAARF directly implements regulatory requirement
- **Enhanced**: HAARF extends regulatory requirement with additional capabilities  
- **Novel**: HAARF addresses capabilities not covered by existing regulations
- **Primary Reference**: Framework serves as foundation (e.g., OWASP AISVS → C3)

## 🏛️ Key Framework Highlights

### FDA Digital Health (84% coverage)
- **C1**: SaMD classification, 510(k) predicate analysis, PCCP
- **C8**: Tool integration, breakthrough device pathway
- **Pathways**: 510(k), De Novo, PMA, Breakthrough Device

### EU AI Act (71% coverage)  
- **High-Risk**: All clinical AI agents qualify under Annex III
- **C4**: Direct Article 14 human oversight implementation
- **C2**: XAI exceeds Article 13 transparency requirements

### OWASP AISVS (56% coverage - Primary Reference)
- **C3.4.1**: "Organizations align with OWASP AISVS as primary cybersecurity guide"
- **Healthcare Adaptations**: All categories adapted for clinical environments
- **C8 Extensions**: Novel tool security not in current AISVS

## 🌐 Multi-Jurisdictional Compliance

HAARF enables simultaneous compliance across jurisdictions:

1. **Foundation**: HAARF Level 2-3 compliance
2. **FDA Focus**: C1 (PCCP), C8 (Tool Use), SaMD
3. **EU Focus**: C4 (Human Oversight), C2 (Transparency), C7 (Equity)  
4. **Health Canada**: C7 (SGBA+), population equity
5. **UK MHRA**: C1 (Real-world evidence), AI Airlock

## 🔧 Implementation Guidance

### Healthcare Organizations
1. Start with C1 three-factor risk assessment
2. Choose primary regulatory jurisdiction
3. Implement C1, C3 (AISVS), C4, C7 for broad coverage
4. Add C8 for tool-enabled agents
5. Document cross-framework compliance

### Regulatory Submissions
- Use mapping evidence for multiple jurisdictions
- Emphasize HAARF enhancements beyond regulatory minimums
- Leverage common evidence requirements
- Plan for international deployment

## 📈 Documentation Evidence

Each mapping includes:
- Specific requirement alignments
- Compliance evidence specifications  
- Regulatory pathway coverage
- Implementation guidance
- Submission documentation requirements

## 🔄 Maintenance

- **Quarterly**: Framework updates review
- **Annual**: Complete mapping refresh  
- **Event-Driven**: Major regulatory changes
- **Community**: Expert feedback integration

---

**Support**: [haarf@quome.site](mailto:haarf@quome.site)

**The HAARF mappings enable confident deployment of healthcare AI agents across global markets while maintaining highest standards of safety, effectiveness, and regulatory compliance.**