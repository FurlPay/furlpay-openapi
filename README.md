# Furlpay OpenAPI Specification

[![license](https://img.shields.io/badge/license-MIT-green)](./LICENSE)

The unified [OpenAPI 3.1](https://spec.openapis.org/oas/v3.1.0) schema for the
[Furlpay](https://furlpay.com) REST API — auth, wallets, cards, swaps,
investing, banking, compliance, and signature-verified webhooks.

Use it to generate typed clients in languages we do not officially ship yet
(Ruby, PHP, Java, C#, ...).

## Generate a client

```bash
# TypeScript (fetch)
npx openapi-generator-cli generate -i openapi.json -g typescript-fetch -o ./furlpay-ts

# Ruby / PHP / Java
npx openapi-generator-cli generate -i openapi.json -g ruby -o ./furlpay-ruby
npx openapi-generator-cli generate -i openapi.json -g php  -o ./furlpay-php
npx openapi-generator-cli generate -i openapi.json -g java -o ./furlpay-java
```

The live spec is also served at [furlpay.com/openapi.json](https://furlpay.com/openapi.json).

Official SDKs: [Node.js](https://github.com/FurlPay/furlpay-node) · CLI: [furlpay-cli](https://github.com/FurlPay/furlpay-cli)

## License

MIT

## Explore in an API client

A ready-made [Postman collection](./collections/furlpay.postman_collection.json)
is generated from this spec (folders per tag, example-resolved request bodies):

- **Postman** — `File > Import` and pick `collections/furlpay.postman_collection.json`,
  or import `openapi.json` directly.
- **Bruno** — `Import Collection > OpenAPI V3` and select `openapi.json`.
- **Insomnia** — `Create > Import From File` and select `openapi.json`
  (Insomnia consumes OpenAPI 3.1 natively).

Set the `baseUrl` variable to `https://furlpay.com` (or your sandbox) after import.
