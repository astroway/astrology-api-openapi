# Astrology API: OpenAPI 3.1 specification

The machine-readable [OpenAPI 3.1](https://spec.openapis.org/oas/v3.1.0) spec of the [AstroWay astrology API](https://api.astroway.info/en/): 804 operations for natal charts, synastry, transits and progressions, Vedic astrology, BaZi and Chinese metaphysics, Human Design, Tarot, Numerology, finished PDF reports and AI interpretations. Generate a typed client in any language, import it into Postman or Insomnia, or point an agent at it.

**[api.astroway.info](https://api.astroway.info/en/)** · [API reference](https://api.astroway.info/en/docs/) · [Pricing](https://api.astroway.info/en/pricing/) · [Get a free key](https://api.astroway.info/dashboard/sign-up) (10,000 credits a month, no card)

## The file

`openapi.json` in this repository is refreshed from production every day by a workflow; `info.version` inside it names the API version it was taken from. The live spec is always at:

```
https://api.astroway.info/v1/openapi.json
```

## Use it

```bash
curl https://api.astroway.info/v1/openapi.json -o openapi.json

# TypeScript types
npx openapi-typescript openapi.json -o astroway.d.ts

# A client in any language openapi-generator supports
npx @openapitools/openapi-generator-cli generate -i openapi.json -g python -o ./client
```

A [Postman collection](https://api.astroway.info/postman/astroway-api.json) is generated from the same spec.

## Official SDKs, no codegen needed

| Stack | Install | Repository |
|---|---|---|
| TypeScript, Node | `npm i @astroway/sdk` | [astroway-typescript](https://github.com/astroway/astroway-typescript) |
| Python | `pip install astroway` | [astroway-python](https://github.com/astroway/astroway-python) |
| PHP | `composer require astroway/sdk` | [astroway-php](https://github.com/astroway/astroway-php), [Laravel](https://github.com/astroway/astroway-php-laravel), [Symfony](https://github.com/astroway/astroway-php-symfony) |
| Go | `go get github.com/astroway/astroway-go` | [astroway-go](https://github.com/astroway/astroway-go) |
| .NET | `dotnet add package Astroway.Sdk` | [astroway-dotnet](https://github.com/astroway/astroway-dotnet) |
| React hooks | `npm i @astroway/react` | [astroway-react](https://github.com/astroway/astroway-react) |
| SVG charts | `npm i @astroway/render` | [astroway-render](https://github.com/astroway/astroway-render) |
| Web components | `npm i @astroway/ui` | [astroway-ui](https://github.com/astroway/astroway-ui) |
| MCP for AI agents | hosted at `https://mcp.astroway.info/mcp`, or `npx -y @astroway/mcp` | [astroway-mcp](https://github.com/astroway/astroway-mcp) |

## Licence

The specification document is MIT, see [LICENSE](LICENSE). The licence covers this file only, not the API service itself, which is provided under its own [terms](https://api.astroway.info/en/terms/).
