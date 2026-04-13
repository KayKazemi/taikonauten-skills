---
description: Review designs for inclusive coverage across disability types — visual, motor, cognitive, and auditory — beyond the minimum WCAG checklist.
argument-hint: "[product, feature, or user journey to review]"
---

# /inclusive-review

Review designs through the lens of different disability types for inclusive coverage.

## Steps

1. **Visual disabilities**: Use the `color-contrast` and `screen-reader-ux` skills to evaluate the experience for users with low vision, colour blindness, and blindness. Check contrast, alt text, screen reader flow, and magnification behaviour.
2. **Motor disabilities**: Use the `keyboard-navigation` and `focus-management` skills to evaluate for users who cannot use a mouse — keyboard-only, switch access, and voice control users. Check target sizes (minimum 24×24px per WCAG 2.5.8), spacing between targets, and drag interactions.
3. **Cognitive disabilities**: Evaluate for users with cognitive, learning, or attention differences.
   - Is the language plain and clear? (Aim for reading age 12 or below for general audiences)
   - Are forms forgiving? (Error messages descriptive, inline validation, no time limits)
   - Is the layout predictable? (Consistent navigation, no unexpected changes of context)
   - Are instructions clear and step-by-step where needed?
4. **Auditory disabilities**: Check that all audio/video content has captions and transcripts. Ensure no important information is conveyed by sound alone.
5. **BFSG context**: Use the `bfsg-compliance` skill to confirm German legal obligations are met for the product.
6. **Summary**: Produce an inclusive design review noting coverage by disability type, gaps, and priority improvements.

## Output

Inclusive design review report structured by disability type, with coverage assessment and prioritised design improvements.
