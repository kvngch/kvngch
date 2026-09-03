```
$ docker compose -f kvngch.yml ps

NAME            IMAGE                        STATUS
business-apps   react-node-php:postgres      Up
mobile          swift-kotlin:compose         Up
desktop         swift-dotnet:tauri           Up
e-commerce      woocommerce-presta:shopify   Up
cms             wordpress-joomla:sanity      Up
```

```yaml
# kvngch.yml

name: kvngch
maintainer: Kévin Gachie, software developer in Marseille
context: E-Corp, a development studio, and its own products

services:

  business-apps:
    scope: scheduling, activity tracking, back offices, portals
    stack: [TypeScript, React, Node, PHP, PostgreSQL]

  mobile:
    scope: iOS and Android, native or cross-platform
    stack: [Swift, Kotlin, Jetpack Compose]
    notes: on-device processing, offline when it matters

  desktop:
    scope: native macOS and Windows applications
    stack: [Swift, dotNET, Tauri]
    notes: Tauri when a web core suits the product

  e-commerce:
    scope: themes and apps, catalogue and inventory sync
    stack: [WooCommerce, PrestaShop, Shopify]
    notes: marketing and ads gateways, ERP connections

  cms:
    scope: content sites and custom plugin development
    stack: [WordPress, Joomla, Sanity, Astro]
    notes: headless where it fits
```

[ecorp-agency.com](https://ecorp-agency.com) · [kvngch.fr](https://kvngch.fr) · [LinkedIn](https://www.linkedin.com/in/kevin-gachie/)
