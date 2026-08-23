# Security Policy

## Supported versions

Security fixes should target the latest published version of Chat to Notion.

## Reporting a vulnerability

Do not disclose suspected vulnerabilities in a public issue.

Use GitHub's **Security** tab and **Report a vulnerability** when private
vulnerability reporting is available. If it is unavailable, contact the
original maintainer using the repository owner's verified contact channel.

Include:

- the affected extension version and browser;
- reproduction steps;
- the impact on Notion data, access tokens, or browsing data;
- the relevant extension page, permission, or server endpoint;
- a minimal proof of concept using test accounts only.

Never include real Notion tokens, cookies, API keys, private conversations, or
database contents. Redact screenshots and logs before sharing them.

## Sensitive areas

Changes involving these areas require particular review:

- Notion OAuth and access-token storage;
- communication with the external server;
- browser host permissions and `webRequest`/`scripting` permissions;
- content extracted from supported LLM websites;
- web-accessible resources;
- logging, analytics, and error reporting.

Use least-privilege permissions, avoid logging secrets, and revoke any
credential that may have been exposed.
