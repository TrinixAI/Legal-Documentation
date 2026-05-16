# AccessScan Third-Party Notices

**Effective Date:** May 16, 2026  
**Provider:** Srdjan Lopez LLC dba Trinix AI  
**Product:** AccessScan

AccessScan may use third-party software, open-source libraries, frameworks, APIs, infrastructure, and services. This page provides practical notice of major third-party technologies and provider categories used or supported by AccessScan.

## 1. Core Application Technologies

AccessScan may include or depend on:

| Technology | Purpose |
|---|---|
| Next.js | Application framework |
| React | User interface framework |
| TypeScript | Application development language |
| Tailwind CSS | Styling and user interface utility framework |
| Node.js | Runtime and API routes |
| Prisma | Database ORM |
| PostgreSQL | Database |
| Playwright | Browser automation for web scanning |
| axe-core | Accessibility rule engine |
| pdfjs-dist | PDF parsing |
| pdf-parse | PDF parser fallback |
| JSZip | DOCX and PPTX parsing support |

## 2. AI Providers and Models

AccessScan may support AI-assisted features through configurable providers, including:

- Anthropic Claude
- Trinix AI
- OpenAI
- Azure OpenAI
- Local or customer-approved models
- Future supported AI providers

AI provider availability depends on configuration, deployment model, customer approval, and applicable agreement.

AI output is guidance only and must be reviewed by qualified humans.

## 3. CI/CD and Developer Integrations

AccessScan may support:

- GitHub Actions
- Jenkins
- Versioned API workflows
- API key authenticated scan triggers
- Command-line CI scripts

Customers are responsible for securing repositories, secrets, build systems, API keys, and connected developer environments.

## 4. Accessibility Standards and References

AccessScan may reference accessibility standards and guidance, including:

- Web Content Accessibility Guidelines
- Revised Section 508 Standards
- WAI-ARIA guidance
- Platform-specific accessibility practices for Drupal, Appian, Salesforce, SharePoint, Microsoft 365, PDF, Word, and PowerPoint workflows

References are used for guidance and issue classification. AccessScan does not certify legal compliance.

## 5. Open-Source Licensing

Some third-party packages may be distributed under open-source licenses. Customers should review the package lockfile, dependency list, and generated SBOM for the exact dependency set used in their deployment.

Recommended pre-release review:

```text
npm ls
npm audit
npm run build
Generate SBOM using your preferred SBOM tool
Review package licenses before enterprise distribution
```

## 6. Third-Party Service Terms

Third-party services may be subject to their own terms, privacy policies, security practices, data retention rules, and usage limits.

Customers are responsible for reviewing and approving third-party services connected to their AccessScan deployment, especially AI providers, hosting providers, storage providers, authentication providers, analytics providers, and CI/CD systems.

## 7. No Endorsement

Reference to third-party products, platforms, standards, or providers does not imply endorsement, sponsorship, certification, or partnership unless expressly stated in writing.

## 8. Contact

Questions about third-party notices may be sent to support@trinix.gg.
