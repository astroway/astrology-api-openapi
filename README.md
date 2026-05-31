# Astrology API — OpenAPI 3.1 Specification

Machine-readable **OpenAPI 3.1 spec** for the [**AstroWay astrology API**](https://api.astroway.info) — a hosted, developer-first **astrology calculation API** powered by the **Swiss Ephemeris** (NASA JPL data). 700+ endpoints, one REST API.

🌐 **[api.astroway.info](https://api.astroway.info)** &nbsp;·&nbsp; 📖 [Docs](https://api.astroway.info/docs/) &nbsp;·&nbsp; 🔑 [Get an API key](https://api.astroway.info)

## What the API calculates

Natal & birth charts · Synastry & compatibility · Transits & progressions · Western & sidereal house systems · **Vedic astrology** (dashas, vargas, panchang, yogas) · **Human Design** · **Tarot** · **Numerology** · AI-generated horoscopes — high-precision planetary positions from the Swiss Ephemeris.

## Use the spec

```bash
# Canonical, always-current spec
curl https://api.astroway.info/v1/openapi.json -o openapi.json

# Generate a typed TypeScript client
npx openapi-typescript openapi.json -o astroway.d.ts

# …or a full SDK in any language
openapi-generator-cli generate -i openapi.json -g python -o ./client
```

The `openapi.json` checked into this repo is a dated snapshot (API v2.74.12). The **live URL above is the source of truth** — fetch it for the latest endpoints.

## Official SDKs (no codegen needed)

TypeScript [`@astroway/sdk`](https://github.com/astroway/astroway-typescript) · Python [`astroway`](https://github.com/astroway/astroway-python) · PHP [`astroway/sdk`](https://github.com/astroway/astroway-php) · React [`@astroway/react`](https://github.com/astroway/astroway-react) · MCP for Claude/Cursor [`@astroway/mcp`](https://github.com/astroway/astroway-mcp)

A hosted alternative to running your own Swiss Ephemeris server — natal chart API, horoscope API and Vedic astrology API in one place.

**[→ Start building at api.astroway.info](https://api.astroway.info)**
