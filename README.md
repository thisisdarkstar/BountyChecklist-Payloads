# BountyChecklist Payloads

External payload collections for the BountyChecklist Chrome Extension.

## Host on GitHub Pages

This repository is designed to be hosted on GitHub Pages. Once hosted, the payloads will be fetched by the BountyChecklist extension dynamically.

### Setup Instructions

1. Create a new GitHub repository named `BountyChecklist-Payloads`
2. Upload the contents of this repository
3. Enable GitHub Pages in repository Settings → Pages → Source: main branch
4. Your payloads URL will be: `https://[username].github.io/BountyChecklist-Payloads/`

### Payload Files

| File | Description |
|------|-------------|
| `payloads/sql-injection.json` | 1000+ SQL Injection payloads |
| `payloads/xss.json` | 800+ XSS payloads |
| `payloads/ssrf.json` | SSRF payloads |
| `payloads/path-traversal.json` | Path traversal payloads |
| `payloads/idor.json` | IDOR parameter manipulation |
| `payloads/command-injection.json` | Command injection payloads |
| `payloads/lfi.json` | Local File Inclusion payloads |
| `payloads/rce.json` | RCE techniques and payloads |
| `payloads/open-redirect.json` | Open redirect payloads |
| `payloads/subdomain-takeover.json` | Subdomain takeover payloads |
| `payloads/wordpress.json` | WordPress testing payloads |
| `payloads/html-injection.json` | HTML injection payloads |
| `payloads/ssti.json` | Server Side Template Injection |
| `payloads/xxe.json` | XXE payloads |
| `payloads/jwt.json` | JWT attack payloads |
| `payloads/graphql.json` | GraphQL testing payloads |

## Payload JSON Format

```json
{
  "name": "SQL Injection",
  "version": "1.0.0",
  "updated": "2026-03-20",
  "category": "sql-injection",
  "description": "SQL Injection payloads for database testing",
  "payloads": [
    "' OR '1'='1",
    "' OR 1=1--",
    "admin'--"
  ]
}
```

## Update Extension Configuration

In `sidebar.js`, update the PAYLOADS_URL to your GitHub Pages URL:

```javascript
const PAYLOADS_URL = 'https://thisisdarkstar.github.io/BountyChecklist-Payloads/payloads/';
```
