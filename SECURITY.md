# Security Policy

## What to report

This repository contains design skills and commands for Claude Code — no application code, no user data, no authentication. That means traditional code vulnerabilities (injection, auth bypass, etc.) don't apply here.

What does matter is **skill content that could cause Claude to behave harmfully or deceptively**. Please report if you find:

- A skill or command that instructs Claude to produce dangerous, misleading, or manipulative output
- Prompt patterns that could be exploited to bypass Claude's safety guidelines
- Instructions that could cause Claude to misrepresent itself or its capabilities to end users

## How to report

Use GitHub's private vulnerability reporting — click **"Report a vulnerability"** on the [Security tab](../../security/advisories/new) of this repository. This keeps the report confidential until it's been reviewed and addressed.

Please don't open a public issue for security concerns — a private report gives us the chance to look into it before it's visible to everyone.

## What to expect

You'll get an acknowledgement within **72 hours**. If the report is valid, we'll work on a fix and credit you in the changelog unless you prefer to stay anonymous.

## Out of scope

The following are not security issues — please use a regular [GitHub issue](../../issues) instead:

- Skill output quality or accuracy
- Missing features or improvement suggestions
- General bugs in documentation or formatting
