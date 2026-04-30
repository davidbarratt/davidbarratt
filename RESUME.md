![dwb](https://files.davidwbarratt.com/dwb.svg)

# David Barratt

Orlando, Florida, United States\
<david@davidwbarratt.com> \
[GitHub](https://github.com/davidbarratt) | [LinkedIn](https://linkedin.com/in/davidbarratt/) | [Drupal](https://www.drupal.org/u/davidwbarratt/)

## Professional Experience

### Flex Technology Co. | Founding Engineer

_May 2024 – Present_

- Migrated PDF generation from PDF Generator to React PDF which significantly improved reliability.
- Created a Consumer portal for merchant's customers to securely access their health and payment documents.
- Migrated the frontend applications to the React Compiler.
- Discovered a bug in WebKit and submitted a patch to Apple.
- Implemented custom fee support end-to-end which allowed merchants to specify any arbitrary fee as part of the checkout process.
- Improved the performance of Playwright tests by ensuring they were correctly sharded by browser.
- Eliminated flaky test failures by enforcing full test isolation in Playwright, improving CI reliability.
- Resolved PHP dependency conflicts in the WordPress plugin by implementing PHP Scoper, preventing fatal PHP errors on merchant sites.
- Created a new Shopify extension to connect users to the reimbursement flow in cases where Shopify prevents third-party payment processors.
- Created a "reimbursement" flow that allowed users to get the documentation they need in order to file for a reimbursement from their HSA/FSA provider.
- Refactored error tracking and reporting in the backend Rust application
- Created the Flex WooCommerce plugin which featured:
  - Payments (Line Items, Taxes, Discounts, Coupons, etc.)
  - Refunds across multiple payment methods
  - Product & Variant sync in the background using Action Scheduler.
  - Webhooks
  - Sentry Telemetry
- Added support for 3DS payment verification
- Added support for embeded (iframe) and popup checkout implementations.
- Provided merchants with the ability to perform multi-payment method refunds from within the merchant dashboard.
- Added subscription support to the merchant dashboard.
- Resolved many timezone related React hydration issues.
- Created a custom authentication flow using Twilio.
- Implemented an A/B testing process and framework using PostHog and Vercel Toolbar that powered real product decisions.
- Ensured the frontend applications utilized TypeScript in the strictest possible settings.
- Refactored the front-end checkout application from a (noncompliant) letter of medical necessity form to an LLM based consultation chat flow using Vercel's AI SDK.
- Added support for "test mode" to all frontend applications.
- Implemented an end-to-end testing system using Playwright
- Implemented schema-first type generation using OpenAPI, JSON Schema, and Zod.
- Created a continuous integration (CI) pipeline using GitHub Actions for all backend and frontend services.

### Drizly, an Uber Company | Senior Staff Engineer, Consumer

_February 2023 – April 2024_

- Collaborated with engineering leaders to simplify Drizly’s technical architecture given an updated business direction.
- Evaluated the performance and developer experience tradeoffs to migrate from Next.js’ Pages Router to App Router.
- Proposed, architected, and achieved consensus on:
  - Migrating from Next.js’ Pages Router to App Router.
  - An implementation for inline content editing within the Scrivito content management system (CMS)
  - Splitting the product taxonomy from the consumer application navigation.
- Implemented a continuous improvement system to encourage engineering teams to progressively migrate to TypeScript.
- Resolved several critical bugs that blocked the migration from Next.js’ Pages Router to App Router.
- Migrated several complex continuous integration (CI) workflows from Jenkins to GitHub Actions.
- Migrated the Docker Compose implementation of the primary web application to utilize Compose Watch which enabled engineers to preview their changes locally in a production-like environment. The feedback loop to preview changes was reduced by 57% when compared to deploying to a staging server.
- Migrated several large parts of Drizly’s JavaScript code base to TypeScript.
- Performed several major upgrades of core system dependencies.

### Drizly, an Uber Company | Staff Software Engineer, Consumer

_November 2020 – February 2023_

- Debugged and resolved a critical issue that prevented customers from being able to checkout due to the Rails session cookie exceeding the browser’s cookie size limit.
- Identified the causes of exceeding Google’s Core Web Vital (CWV) metric thresholds and proposed solutions.
- Debugged and resolved a critical issue with Hypernova that caused the Cumulative Layout Shift (CLS) metric to far exceed Google’s threshold.
- Created a technical roadmap for the primary consumer web application.
- Instrumented geolocation services usage, which exposed a large-scale data harvesting operation. Blocking the operation saved the company $380,000 each year by reducing the geolocation service costs by 42%.
- Determined that migrating the primary consumer web application from the legacy code base to Next.js, without any additional optimizations, would reduce the Time to First Byte (TTFB) by 39% and Largest Contentful Paint (LCP) by 24%.
- Proposed, architected, and achieved consensus on:
  - A service to retrieve and cache data from the Scrivito content management system (CMS) API
  - A migration strategy for migrating Drizly’s client facing APIs to an abstracted service-oriented architecture.
  - A comprehensive edge caching strategy utilizing bubbling cache tags from dependent services to store content with an infinite time to live (TTL) while invalidating on dependency update.
  - A cache invalidation service to invalidate dynamic HTTP responses from an edge cache.
  - An incremental migration strategy from the existing legacy code base to the Next.js framework.
  - A solution to reduce the latency of some data science services to near zero by migrating the services to a portable executable.
  - A mechanism to prevent the Web Application Firewall (WAF) from blocking legitimate customers from completing the checkout process.
- Documented and advocated best practices across several engineering teams and wrote a best practice guide for:
  - Caching dynamic HTTP responses in an edge cache.
  - Persisting client-side state
  - Using TypeScript
  - Testing JavaScript & TypeScript code
- Designed and implemented an integration strategy between Next.js and the Scrivito content management system (CMS).
- Mentored a mid-level software engineer using pair programming and assisted in teaching them the technical skills required for a promotion to senior engineer.
- Created a cache proxy using Cloudflare Workers to cache API responses from the Scrivito API which reduced the latency of these requests from the client applications by 80%.
- Debugged and created a work-around for a critical error in production that was caused by a browser vendor’s incorrect implementation of an existing specification.
- Migrated multiple complex applications into multi-platform Docker containers.

### Wikimedia Foundation, the stewards of Wikipedia | Senior Software Engineer, Anti-Harassment

_May 2017 – October 2020_

- Implemented new features in MediaWiki that allowed users on Wikipedia to:
  - Prevent being emailed by specific users.
  - Issue partial blocks on specific pages or namespaces rather than the entire wiki.
  - Perform investigations of users or IP address to address harassment.
- Created a GraphQL extension for MediaWiki as a proof of concept to allow engineers to make distributed queries across all of Wikimedia’s wikis.
- Created and maintained Docker’s official MediaWiki container image.

### iHeartMedia | Software Engineer, RadioEdit Platform

_January 2017 - May 2017_

Designed and developed features in TypeScript utilizing the Angular framework for the RadioEdit custom content management system (CMS).

### Golf Channel | Senior Software Engineer, GolfChannel.com

_November 2014 - January 2017_

Led the migration GolfChannel.com from Drupal 7 to a decoupled Drupal 8 and Node.js application while overseeing the implementation of all CMS features.

### Camna, LLC | Senior Web Developer

_October 2012 - October 2014_

Implemented custom designs and wrote custom plugins for new or existing websites built on Drupal, WordPress, ExpressionEngine, CodeIgniter, CiviCRM, Drupal Commerce and WooCommerce.

### RELEVANT Media Group | Digital Development Director

_January 2010 - October 2012_

Led the migration from Joomla! to Drupal 7 and developed forty custom plugins to achieve the desired functionality including a custom subscription management solution.

## Education

### University of Central Florida | Master of Business Administration

_May 2027_

Learning to apply advanced theoretical concepts and knowledge from all functional areas of business through an analytical, decision-making process that focuses on solving practical problems.

### University of Central Florida | Graduate Certificate in Entrepreneurship

_May 2020_

Learned how to recognize business opportunities, formulate solutions to customer problems, design business models, and deliver results.

### University of Central Florida | Bachelor of Arts in Digital Media

_May 2011_

Learned the foundations of user experience, pseudocode, information architecture, semantic content, structured content, and accessibility; and practically implemented these foundations into complex web applications.
