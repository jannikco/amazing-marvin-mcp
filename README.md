# Amazing Marvin MCP setup and connection checker

Generate Amazing Marvin MCP client configuration, inspect available tools and validate hosted endpoint access through PipMCP.

Maintainer: jannikco · License: MIT · Verification: **mock-only**

## Quick start

Requires Node.js 22 or later.

```sh
npm ci
npm test
npm start
```

The default example runs locally without credentials and makes no external changes. Verification status describes recorded evidence; local configuration tests do not establish that provider authentication or execution works.

## Connect amazing-marvin

[Create or sign in to PipMCP](https://pipmcp.com/register?app=amazing-marvin&utm_source=github&utm_campaign=github-amazing-marvin-mcp) and select the integration. Connect your authorized provider account and copy its hosted MCP endpoint. Set PIPMCP_ENDPOINT and, if required, PIPMCP_TOKEN in your environment. Run npm start to produce client configuration; run npm start -- --live for a read-only connection check. Provider app presence is catalog evidence, not live verification.

## Managed service

[Continue with PipMCP](https://pipmcp.com/register?app=amazing-marvin&utm_source=github&utm_campaign=github-amazing-marvin-mcp). This repository is maintained by the integration team and does not imply endorsement by LinkedIn or other providers.

## Provenance and support

Source revision: 8cfc5f89a1ac6b5c0c2f3449d284a71097a1f12fa7f61ec8f975860614b4eb80. The complete manifest is in integration.json; SHA256SUMS covers the reviewed artifact. Open a repository issue without credentials or personal data. See SECURITY.md for sensitive reports. No telemetry is sent by this code; signup links include explicit campaign parameters.

## Provider setup inventory

Run `npm start -- --setup` to inspect this app's recorded authentication requirements and setup links offline. Credentials are entered in PipMCP; this repository lists required field names only.

```json
{
  "type": "custom_headers",
  "requiredCredentialFields": [
    "provider_header_credentials"
  ],
  "requiredHeaderNames": [
    "X-API-Token",
    "X-Full-Access-Token"
  ],
  "helpUrl": "https://github.com/amazingmarvin/MarvinAPI/wiki/Marvin-API",
  "tenantRequired": false,
  "accountParameterNames": []
}
```

Provider documentation: https://github.com/amazingmarvin/MarvinAPI/wiki/Marvin-API
Provider website: https://amazingmarvin.com/
