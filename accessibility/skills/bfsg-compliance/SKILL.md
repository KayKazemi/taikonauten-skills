---
name: bfsg-compliance
description: Meet German BFSG (Barrierefreiheitsstärkungsgesetz) accessibility requirements for digital products and services. Use when designing or auditing products for the German market.
---

# BFSG Compliance

Meet Germany's Barrierefreiheitsstärkungsgesetz (BFSG) — the national law transposing the EU Web Accessibility Directive and European Accessibility Act into German law.

## What You Do

You help teams understand and apply BFSG requirements to digital products — translating the legal framework into concrete design and development requirements.

## Legal Context

- **BFSG** came into force on **28 June 2025** for new products and services. It applies to private sector businesses (unlike the earlier BITV, which only covered public sector).
- **Scope**: Consumer-facing digital products and services, including websites, mobile apps, e-commerce, digital services, and self-service terminals.
- **Standard**: Compliance is measured against **EN 301 549**, which references **WCAG 2.1 AA** as the baseline, and incorporates additional requirements.
- **Enforcement**: Enforced via market surveillance authorities (Marktüberwachungsbehörden). Non-compliance can result in injunctions and fines.

## What is Required

1. **WCAG 2.1 AA conformance** for all digital interfaces — see `wcag-compliance` skill for details
2. **Accessibility statement (Barrierefreiheitserklärung)**: A publicly available statement declaring the accessibility status, known limitations, and a contact for accessibility requests
3. **Feedback mechanism**: Users must be able to report accessibility barriers and receive a response
4. **Accessible documentation**: Any documentation provided with the product must also be accessible

## Accessibility Statement (Barrierefreiheitserklärung) Requirements

- Scope of the statement (which product/service it covers)
- Level of conformance (full, partial, non-conformant)
- Non-accessible content: list of known issues and reasons
- Alternatives: what accessible alternatives are available
- Contact information for accessibility requests
- Enforcement body contact (for escalation)
- Date of last assessment

## Practical Design Implications

- **WCAG 2.1 AA is the floor** — design and test to this standard across all user journeys
- **Mobile accessibility**: Requirements apply equally to native apps (iOS and Android)
- **Third-party content**: You are responsible for embedded third-party content — check that plugins, maps, and widgets are accessible
- **Procurement**: When commissioning third-party development, BFSG compliance must be a contractual requirement

## Audit and Documentation

- Conduct a formal WCAG 2.1 AA audit before launch
- Document non-conformances and remediation timelines
- Publish the accessibility statement and keep it updated
- Establish an internal process for responding to accessibility complaints within 30 days

## Further Reading

- BFSG — Official German Law Text (bgbl.de)
- EN 301 549 — ETSI Standard
- WCAG 2.1 — W3C
- EU Web Accessibility Directive (2016/2102/EU)
- European Accessibility Act (EAA) 2019/882
