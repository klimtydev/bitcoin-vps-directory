# Bitcoin VPS — Bitcoin & Crypto VPS Directory

Compare VPS hosting providers that accept Bitcoin and other cryptocurrencies. [Bitcoin VPS](https://bitcoin-vps.net/) brings provider descriptions, hosting plans, server locations and privacy-related features into one searchable catalog.

Find a server for a personal VPN, proxy, application or self-hosted service without opening dozens of hosting websites just to compare the basics.

**[Compare VPS plans](https://bitcoin-vps.net/) · [Browse providers](https://bitcoin-vps.net/providers)**

## What you can compare

- **Prices and resources:** monthly comparison prices in USD, CPU, RAM, storage and disk type.
- **Server locations:** filter by one or several countries.
- **No-KYC options:** find providers listed as not requiring identity verification. Cryptocurrency payment support and no-KYC signup are separate properties.
- **Network and privacy features:** distinguish IPv6-only plans, privacy-focused providers and recorded hosting policies.
- **Payment requirements:** identify providers that require an initial card payment before cryptocurrency payments become available.
- **Provider profiles:** read short descriptions and explore each provider's listed plans.

IPv6-only plans are hidden by default in plan search. You can include them when an IPv6-only server suits your use case.

The interface is available in [English](https://bitcoin-vps.net/) and [Russian](https://bitcoin-vps.net/ru).

## Public catalog API

The public, read-only API lets you search offers, find providers and retrieve provider profiles with their plans. No API key is required for these catalog endpoints.

```sh
curl --get 'https://bitcoin-vps.net/api/catalog/search' \
  --data-urlencode 'noKyc=yes' \
  --data-urlencode 'budget=5' \
  --data-urlencode 'hideIpv6Only=true'
```

This searches for no-KYC offers with a monthly comparison price of up to USD 5 and excludes IPv6-only plans. The response separates matching offers from suggestions whose resources are not confirmed.

- [API documentation](docs/catalog-api.md)
- [Live OpenAPI specification](https://bitcoin-vps.net/api/catalog/openapi.json)
- [ARD discovery manifest](https://bitcoin-vps.net/.well-known/ard.json)

Compatible browsers and agents can also use the site's experimental WebMCP integration. The HTTP API works independently of browser support.

## Report a correction or suggest a provider

Use this repository's Issues to report an outdated price, incorrect location or provider detail, or to suggest a cryptocurrency-friendly VPS provider.

Please include the provider name, a link to the relevant page on Bitcoin VPS, the official source URL and a short explanation of the change. For a listing suggestion, include server locations and cryptocurrency payment options. Do not include account credentials or personal information.

## About the data

Original plan prices are kept in the provider's currency and converted to USD for comparison. A monthly comparison figure does not necessarily mean that the provider offers a one-month billing period. Check the provider's current pricing and availability before ordering.

Provider policies are recorded separately: accepting Bitcoin does not by itself establish no-KYC signup or permission for a particular hosting use case.

See [how providers are selected](https://bitcoin-vps.net/how-we-choose), [the project's mission and privacy information](https://bitcoin-vps.net/privacy-and-mission), and [project updates](https://bitcoin-vps.net/updates).

This repository contains project information and public API documentation. The website's application source code is not published here.
