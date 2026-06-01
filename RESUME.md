![dwb](https://files.davidwbarratt.com/dwb.svg)

# David Barratt

Orlando, Florida, United States  
<david@davidwbarratt.com>  
[GitHub](https://github.com/davidbarratt) | [LinkedIn](https://linkedin.com/in/davidbarratt/) | [Drupal](https://www.drupal.org/u/davidwbarratt/)

## Professional Summary

Founding Engineer (Senior Staff) with 15+ years building high-performance web applications in TypeScript, React/Next.js, Node.js, PHP/Drupal, and cloud infrastructure (Docker, CI/CD, edge caching). Architected systems that cut latency by 80%, saved $380K/year in infrastructure costs, and shipped to millions of users. MBA Candidate (Expected 2027) with a Graduate Certificate in Entrepreneurship, combining technical depth with a business-first approach to product decisions.

## Technical Skills

- **Languages & Runtimes:** TypeScript, JavaScript, PHP, Node.js, Rust, Ruby, SQL
- **Frameworks:** React, Next.js, Angular, Ruby on Rails
- **Cloud Services:** Amazon Web Services (AWS), Cloudflare Workers, Vercel
- **CMS & E-commerce:** Drupal, WordPress, WooCommerce, Shopify, Acquia
- **Data & Analytics:** Snowflake, Metabase, PostHog
- **Observability:** Sentry, New Relic
- **Platforms & Tools:** Docker, GitHub Actions, Varnish
- **Testing:** Playwright, Jest, Vitest, PHPUnit
- **APIs & Standards:** GraphQL, OpenAPI, Zod
- **Practices:** CI/CD, Edge Caching, A/B Testing

## Professional Experience

### Flex Technology Co. | Founding Engineer
*May 2024 – Present*

- Built an AI-powered checkout consultation flow using LLM-driven dialogue to determine HSA/FSA eligibility, replacing static forms.
- Built the Flex WooCommerce plugin from scratch and shipped it to WordPress.org with an automated release pipeline (builds, GitHub Releases, SVN deployment).
- Created the consumer portal where HSA/FSA cardholders view orders, receipts, and Letters of Medical Necessity.
- Fixed a critical IDOR vulnerability in the WooCommerce order-completion endpoint, preventing unauthorized order manipulation.
- Hardened the CI/CD pipeline to prevent untested code from reaching production.
- Designed a custom fee system with proportional line-item distribution, letting merchants attach arbitrary fees while preserving correct coupon discounting.
- Created a self-contained development container enabling Claude Code to operate as an autonomous engineering agent across Rust, Node.js, and PHP.

### Drizly, an Uber Company | Senior Staff Engineer, Consumer
*February 2023 – April 2024*

- Led architectural simplification of Drizly's technical stack following an updated business direction.
- Evaluated performance and developer experience tradeoffs and led the migration from Next.js Pages Router to App Router.
- Architected and drove adoption of:
  - An implementation for inline content editing within the Scrivito CMS.
  - Splitting the product taxonomy from the consumer application navigation.
- Implemented a continuous improvement system to progressively migrate engineering teams to TypeScript.
- Migrated complex CI workflows from Jenkins to GitHub Actions.
- Migrated the Docker Compose setup to use Compose Watch, reducing the feedback loop for previewing changes by 57% vs. deploying to staging.

### Drizly, an Uber Company | Staff Software Engineer, Consumer
*November 2020 – February 2023*

- Debugged and resolved a critical checkout-blocking issue caused by the Rails session cookie exceeding the browser's cookie size limit.
- Resolved a critical Hypernova issue causing Cumulative Layout Shift (CLS) to far exceed Google's threshold.
- Instrumented geolocation services usage, exposing a large-scale data harvesting operation. Blocking it saved $380,000/year (42% cost reduction).
- Determined that migrating from legacy codebase to Next.js alone would reduce TTFB by 39% and LCP by 24%.
- Architected and drove adoption of:
  - A service to retrieve and cache data from the Scrivito CMS API.
  - A migration strategy for client-facing APIs to an abstracted service-oriented architecture.
  - A comprehensive edge caching strategy using bubbling cache tags for infinite TTL with dependency-based invalidation.
  - A cache invalidation service for dynamic HTTP responses from edge cache.
  - An incremental migration strategy from legacy codebase to Next.js.
  - Reducing data science service latency to near-zero by migrating to portable executables.
  - Preventing the WAF from blocking legitimate customers at checkout.
- Created a Cloudflare Workers cache proxy for Scrivito API responses, reducing client-side request latency by 80%.
- Authored 4+ engineering guides on edge caching, client-side state, TypeScript, and JS/TS testing; established team-wide best practices.
- Designed and implemented the integration strategy between Next.js and the Scrivito CMS.
- Mentored a mid-level engineer through pair programming, supporting their promotion to senior engineer.
- Debugged and worked around a critical production error caused by a browser vendor's incorrect implementation of a web specification.

### Wikimedia Foundation | Senior Software Engineer, Anti-Harassment
*May 2017 – October 2020*

- Implemented MediaWiki features enabling Wikipedia users to block email from specific users, issue partial blocks on pages/namespaces, and investigate users/IPs for harassment.
- Created a GraphQL extension for MediaWiki as a proof of concept for distributed queries across all Wikimedia wikis.
- Created and maintained Docker's official MediaWiki container image.

### iHeartMedia | Software Engineer, RadioEdit Platform
*January 2017 – May 2017*

- Designed and developed TypeScript/Angular features for the RadioEdit custom CMS.

### Golf Channel | Senior Software Engineer, GolfChannel.com
*November 2014 – January 2017*

- Led the migration of GolfChannel.com from Drupal 7 to a decoupled Drupal 8 and Node.js application, overseeing all CMS feature implementations.

### Camna, LLC | Senior Web Developer
*October 2012 – October 2014*

- Implemented custom designs and wrote plugins for websites built on Drupal, WordPress, ExpressionEngine, CodeIgniter, CiviCRM, Drupal Commerce, and WooCommerce.

### RELEVANT Media Group | Digital Development Director
*January 2010 – October 2012*

- Led the migration from Joomla! to Drupal 7 and developed 40+ custom plugins including a subscription management solution.

## Open Source Projects

- **Flex HSA/FSA Payments WooCommerce Plugin** ([source](https://github.com/joinflexhealth/woocommerce)) — Built and published to WordPress.org with automated CI/CD pipeline.
- **MediaWiki Docker Image** ([source](https://github.com/wikimedia/mediawiki-docker)) — Created and maintain Docker's official MediaWiki container image, used by developers and organizations worldwide.
- **MediaWiki GraphQL Extension** ([source](https://github.com/wikimedia/mediawiki-extensions-GraphQL)) — Built a GraphQL extension enabling distributed queries across all Wikimedia wikis.
- **Phabricator Docker Image** ([source](https://github.com/phabricator-docker/phabricator)) — Created the official Docker container image for Phabricator.
- **Microsoft OneDrive CLI** ([source](https://github.com/onedrivejs/onedrive)) — Node.js CLI tool for OneDrive file management.
- **RSS Reader (Chickaree)** ([source](https://github.com/chickaree)) — Next.js-based RSS reader application.
- **Drupal Modules** — Authored 6+ published modules including Display Field Copy, Menu Normalizer, REST Menu Tree, and Composer Vendor Autoload.

## Education

- **Master of Business Administration** — University of Central Florida (May 2027)
- **Graduate Certificate in Entrepreneurship** — University of Central Florida (May 2020)
- **Bachelor of Arts in Digital Media** — University of Central Florida (May 2011)
