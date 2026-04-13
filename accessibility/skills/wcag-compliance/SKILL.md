---
name: wcag-compliance
description: Apply WCAG 2.1 and 2.2 success criteria at AA and AAA levels to digital products. Use as the foundation for any accessibility review or inclusive design process.
---

# WCAG Compliance

Apply the Web Content Accessibility Guidelines systematically to ensure digital products are perceivable, operable, understandable, and robust.

## What You Do

You help design teams understand, apply, and audit against WCAG 2.1 and 2.2 success criteria — translating legal and technical requirements into practical design decisions.

## The Four Principles (POUR)

- **Perceivable**: Information and UI components must be presentable in ways users can perceive (text alternatives, captions, contrast, adaptable layout)
- **Operable**: UI components and navigation must be operable (keyboard accessible, enough time, no seizure triggers, navigable)
- **Understandable**: Information and UI operation must be understandable (readable, predictable, input assistance)
- **Robust**: Content must be robust enough to be interpreted by assistive technologies (compatible, parseable)

## Conformance Levels

- **A**: Minimum — failure at this level makes the product unusable for some users
- **AA**: Standard — required by most regulations including EU BFSG, EN 301 549, and Section 508
- **AAA**: Enhanced — aspirational; not required globally but worth targeting for key journeys

## Key WCAG 2.2 Updates (new criteria)

- **2.4.11 Focus Appearance (AA)**: Focus indicators must meet minimum size and contrast requirements
- **2.4.12 Focus Appearance (AAA)**: Enhanced focus indicator specifications
- **2.5.3 Label in Name (A)**: Accessible name must contain the visible label text
- **3.2.6 Consistent Help (A)**: Help mechanisms must appear in the same location across pages
- **3.3.7 Redundant Entry (A)**: Don't ask users to re-enter information already provided
- **3.3.8 Accessible Authentication (AA)**: No cognitive tests required to authenticate

## Practical Application

- Run WCAG checks at design stage, not just in QA — it's cheaper to fix in Figma than in production
- Use automated tools (axe, Lighthouse) for the 30% of issues they catch; manual testing for the rest
- Test with real assistive technology: NVDA + Chrome (Windows), VoiceOver + Safari (Mac/iOS)

## Further Reading

- WCAG 2.2 — W3C
- Inclusive Design Principles — Henny Swan et al.
