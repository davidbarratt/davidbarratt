![dwb](https://files.davidwbarratt.com/dwb.svg)

# David Barratt

Orlando, Florida, United States  
<david@davidwbarratt.com>  
[GitHub](https://github.com/davidbarratt) | [LinkedIn](https://linkedin.com/in/davidbarratt/) | [Drupal](https://www.drupal.org/u/davidwbarratt/)

## Professional Summary

Founding Engineer (Senior Staff). 16+ years building web applications in TypeScript, React/Next.js, Node.js, PHP/Drupal, and cloud infrastructure (Docker, CI/CD, edge caching). Cut latency 80%, saved $380K/year in infrastructure costs, and lifted checkout conversion 6.8% on products serving millions of users. MBA Candidate (Expected 2027) with a Graduate Certificate in Entrepreneurship.

## Technical Skills

- **Languages & Runtimes:** TypeScript, JavaScript, PHP, Node.js, Rust, Ruby, SQL
- **Frameworks:** React, Next.js, Angular, Ruby on Rails, Zod
- **Cloud Services:** Amazon Web Services (AWS), Cloudflare Workers, Vercel, Acquia
- **CMS & E-commerce:** Drupal, WordPress, WooCommerce, Shopify
- **Databases:** PostgreSQL, MariaDB, MySQL, SQLite, Redis
- **Data & Analytics:** Snowflake, Metabase, PostHog
- **Observability:** Sentry, New Relic
- **Infrastructure & DevOps:** Docker, GitHub Actions, Varnish
- **Testing:** Playwright, Jest, Vitest, PHPUnit, PHPStan
- **APIs & Standards:** GraphQL, OpenAPI
- **Practices:** CI/CD, Edge Caching, A/B Testing

## Professional Experience

### Flex Technology Co. | Founding Engineer
*May 2024 – Present*

- Replaced the static HSA/FSA eligibility form with a checkout consultation flow driven by LLM dialogue.
- Ran an A/B test of the checkout diagnosis flow and rolled out the winning variant: checkout conversion up 6.8%, disqualifications down 69%.
- Designed and built a custom fee system that distributes fees proportionally across line items in the Rust backend, WooCommerce plugin, checkout, and merchant dashboard. Partners can attach arbitrary fees without breaking coupon discounting.
- Kept payments correct through a 3× traffic step-up by fixing race conditions that double-charged or blocked customers: duplicate idempotency keys, a 3DS timing flaw, and expired checkouts on backgrounded tabs.
- Built the consumer portal where HSA/FSA cardholders manage orders, receipts, invoices, refunds, and Letters of Medical Necessity. Portal users repurchased within 60 days at 19.1%, against 12.2% for non-portal buyers.
- Wrote the Flex WooCommerce plugin from scratch and shipped it to WordPress.org with an automated release pipeline covering builds, GitHub Releases, and SVN deployment. Fixed a critical IDOR vulnerability in its order-completion endpoint that allowed unauthorized order manipulation.
- Built a self-contained development container so Claude Code could work as an autonomous engineering agent across Rust, Node.js, and PHP.

### Drizly, an Uber Company | Senior Staff Engineer, Consumer
*February 2023 – April 2024*

- Led the simplification of Drizly's stack after a change in business direction.
- Weighed performance against developer experience, then led the migration from Next.js Pages Router to App Router.
- Architected and drove adoption of:
  - Inline content editing in the Scrivito CMS.
  - A split between the product taxonomy and consumer application navigation.
- Set up a continuous improvement process that moved engineering teams onto TypeScript.
- Replaced Jenkins CI with GitHub Actions.
- Moved the Docker Compose setup to Compose Watch. Previewing changes got 57% faster than deploying to staging.

### Drizly, an Uber Company | Staff Software Engineer, Consumer
*November 2020 – February 2023*

- Fixed a checkout-blocking bug: the Rails session cookie had grown past the browser's cookie size limit.
- Tracked down a Hypernova issue that pushed Cumulative Layout Shift (CLS) far past Google's threshold.
- Instrumented geolocation service usage. That exposed a large-scale data harvesting operation; blocking it saved $380,000/year, a 42% cost reduction.
- Measured that migrating the legacy codebase to Next.js alone would cut TTFB by 39% and LCP by 24%.
- Architected and drove adoption of:
  - A service to fetch and cache data from the Scrivito CMS API.
  - A migration path for client-facing APIs onto an abstracted service-oriented architecture.
  - An edge caching strategy using bubbling cache tags for infinite TTL with dependency-based invalidation.
  - A service that invalidates dynamic HTTP responses in edge cache.
  - An incremental migration strategy from the legacy codebase to Next.js.
  - Portable executables for the data science service, which took its latency to near zero.
  - A fix for the WAF blocking legitimate customers at checkout.
- Put the Scrivito API behind a Cloudflare Workers cache proxy. Client-side request latency dropped 80%.
- Wrote 4+ engineering guides on edge caching, client-side state, TypeScript, and JS/TS testing; these became the team's conventions.
- Designed and built the integration between Next.js and the Scrivito CMS.
- Mentored a mid-level engineer through pair programming. They made senior engineer.
- Worked around a production error caused by a browser vendor's wrong implementation of a web specification.

### Wikimedia Foundation | Senior Software Engineer, Anti-Harassment
*May 2017 – October 2020*

- Shipped MediaWiki features that let Wikipedia users block email from specific users, issue partial blocks on pages/namespaces, and investigate users/IPs for harassment.
- Wrote a GraphQL extension for MediaWiki to prove out distributed queries across all Wikimedia wikis.
- Built and maintained Docker's official MediaWiki container image.

### iHeartMedia | Software Engineer, RadioEdit Platform
*January 2017 – May 2017*

- Built TypeScript/Angular features for the RadioEdit custom CMS.

### Golf Channel | Senior Software Engineer, GolfChannel.com
*November 2014 – January 2017*

- Led GolfChannel.com's migration from Drupal 7 to a decoupled Drupal 8 and Node.js stack, covering all CMS feature work.

### Camna, LLC | Senior Web Developer
*October 2012 – October 2014*

- Built custom designs and wrote plugins for sites on Drupal, WordPress, ExpressionEngine, CodeIgniter, CiviCRM, Drupal Commerce, and WooCommerce.

### RELEVANT Media Group | Digital Development Director
*January 2010 – October 2012*

- Led the migration from Joomla! to Drupal 7 and wrote 40+ custom plugins, including a subscription management system.

## Open Source Projects

- **Flex HSA/FSA Payments WooCommerce Plugin** ([source](https://github.com/joinflexhealth/woocommerce)) — published on WordPress.org with an automated CI/CD pipeline for builds and releases.
- **MediaWiki Docker Image** ([source](https://github.com/wikimedia/mediawiki-docker)) — Docker's official MediaWiki container image.
- **MediaWiki GraphQL Extension** ([source](https://github.com/wikimedia/mediawiki-extensions-GraphQL)) — a GraphQL extension for distributed queries across all Wikimedia wikis.
- **Phabricator Docker Image** ([source](https://github.com/phabricator-docker/phabricator)) — the official Docker container image for Phabricator.
- **Microsoft OneDrive CLI** ([source](https://github.com/onedrivejs/onedrive)) — a Node.js CLI for OneDrive file management.
- **RSS Reader (Chickaree)** ([source](https://github.com/chickaree)) — an RSS reader built on Next.js.
- **Drupal Modules** — 6+ published modules, including Display Field Copy, Menu Normalizer, REST Menu Tree, and Composer Vendor Autoload.

## Education

- **Master of Business Administration** - University of Central Florida (May 2027)
- **Graduate Certificate in Entrepreneurship** - University of Central Florida (May 2020)
- **Bachelor of Arts in Digital Media** - University of Central Florida (May 2011)
