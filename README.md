# ISO 6346 Container & Chassis Check-Digit Validator — TypeScript / JavaScript Client

[![npm version](https://img.shields.io/npm/v/@noor-mkdad/container-validator-client.svg)](https://www.npmjs.com/package/@noor-mkdad/container-validator-client)
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/57865358-8bafe64c-1441-4fe3-ba7a-2d60bdeb7dc5)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![RapidAPI Listing](https://img.shields.io/badge/RapidAPI-Dedicated%20Listing-blueviolet)](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/iso-6346-container-chassis-check-digit-validator)

Official zero-dependency, ultra-lightweight Node.js & browser client for **ISO 6346 Container & Chassis Check-Digit Validator**.

> Ultra-fast MOD-11 check digit validator and ISO 6346 size/type decoder for intermodal shipping containers, chassis, and trailers.

> 🔑 **Get your Dedicated API Key:** [Subscribe to ISO 6346 Container & Chassis Check-Digit Validator on RapidAPI](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/iso-6346-container-chassis-check-digit-validator)

---

## 🚀 Installation

```bash
npm install @noor-mkdad/container-validator-client
# or
pnpm add @noor-mkdad/container-validator-client
# or
yarn add @noor-mkdad/container-validator-client
```

---

## ⚡ Quickstart

```typescript
import { ContainerValidatorClient } from '@noor-mkdad/container-validator-client';

// Pass your RapidAPI key for authenticated edge access
const client = new ContainerValidatorClient({
  apiKey: process.env.RAPIDAPI_KEY // Get key from https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/iso-6346-container-chassis-check-digit-validator
});

async function run() {
  const result = await client.validate({
    // Enter validation payload
  });

  if (result.success) {
    console.log('Result:', result.data);
  } else {
    console.error('Error:', result.error);
  }
}

run();
```

---

## 📚 API Reference

### `new ContainerValidatorClient(config)`
- `config.apiKey` *(optional)*: RapidAPI Key (`x-rapidapi-key`).
- `config.baseUrl` *(optional)*: Direct edge worker override URL.

### `client.validate(payload)`
Dispatches standard validation / parse request with sub-5ms latency.

### `client.getHealth()`
Checks edge isolate health and responsiveness.

---

## 🔗 Links
- 📖 [RapidAPI Documentation & Key](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/iso-6346-container-chassis-check-digit-validator)

## 📄 License
MIT © Noor Mkdad
