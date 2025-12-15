# Web-Integrity-Checker
A lightweight web auditor that crawls multiple pages, detects broken links, performs basic accessibility checks, and generates machine‑readable reports (JSON/CSV). Designed for developers and QA teams to integrate into CI/CD pipelines and improve site quality.
Features
- Detects broken links on any website  
- Validates alt text on images  
- Checks heading structure  
- Crawls multiple pages  
- Generates JSON reports  
- Easy to run locally or via CI 

Tech Stack
- Playwright  
- TypeScript  
- Node.js  
- JSON Reporting  

├── tests/                     # Test specifications
│ check-link.spec.ts         # Unit tests for broken link detection
│ accessibility.spec.ts      # Unit tests for accessibility checks
│ crawl-sitemap.spec.ts      # Unit tests for multi-page crawling

├── helpers/                      # Core helper modules
│ crawler.ts                # Handles page crawling logic
│ accessibility.ts          # Performs accessibility validations
│ reporter.ts               # Generates machine-readable reports

├── reports/                     # Generated output reports
│ links-broken.json             # Report of detected broken links
│ accessibility-report.json     # Report of accessibility findings
│ links-valid.json              # Report of valid links
│ accessibility-error.json      # Report of unaccessible findings
│ crawling-report.json          # Report of crawling findings

1.npm install
2.npx playwright install
3.npx playwright test
4.npx playwright test --last-failed



