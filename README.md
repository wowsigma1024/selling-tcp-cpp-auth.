# selling-tcp-cpp-auth.
Server-side:

Full JWT management with rotating secrets: multi-kid parsing, issuer/audience/enforced expiration, /api-friendly session endpoints, and route protection middleware.
Self-hosted panel framework that ensures dedicated schema, stores plan/payment/credential/activity data, exposes helpers for plan CRUD (durations, duration prices/Stripe IDs, tier normalization, feature arrays), payment integration tracking (Coinbase/Stripe/Cash App/PayPal/manual), panel activity/manual updates, subscription fetch/deliver flows, and credential rotation/validation.
Application APIs let owners fetch/delete apps plus upload/manage validated files with owner/reseller access checks, plan uniqueness enforcement, PE header verification, PNG overrides, Cloudflare R2 storage, and metadata persistence that updates plan defaults.
Client/website:

Landing experience with loader, hero, showcase, stats, pricing tiers (Developer/Production/Enterprise), CTA, and pricing checkout button hookup.
Security-focused messaging (AES-256, SSL/TLS, HWID spoof detection, AI monitoring, VMP builds) plus visual badges.
Features exposed via CheckoutButton, pricing list, login/register navigation, and footer links.
Infrastructure/ops:

PostgreSQL pool usage for all APIs, Cloudflare R2 storage with typed content dispositions, environment configurable file-size cap, and helper utilities for plan sanitization/normalization
