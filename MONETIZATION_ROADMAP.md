# Retro Relay Browser — Optional Revenue Systems

**Status:** Approved for development, not shipped. **Current build:** Preview 3 is unchanged. No payment, advertising, or affiliate account has been configured.

## Principles
- Keep the browser free; core themes, browsing, and gaming functions remain free.
- No pop-ups, injected ads into third-party pages, hidden tracking, resale of browsing history, paid ranking disguised as editorial picks, or forced default-search changes.
- Opt-in/visible placements with clear **Sponsored**, **Affiliate link**, or **Support** disclosures.
- No live payment credentials, secret tokens or private user data in the public repository.
- User consent for any analytics; respect disabled telemetry and privacy controls.
- Staff/moderator approval before a developer spotlight goes public.

## Track A — Indie Developer Spotlight
Existing Indie Discovery submission features are the starting point; do not break Create Submission, Submission Drafts, Import Drafts, Import Review Profile or Export Showcases.

**MVP**: Developers submit title, developer/studio, description, genre, release status, official URLs, artwork ownership/license and contact email; clear consent/terms and moderation queue. Unpaid standard submission remains free. Optional paid placements are separate, visibly labeled **Sponsored**, dated, and never presented as independent reviews or guaranteed high rankings.

**Starter package idea (not an accepted rate):** $50 for one week of a labeled spotlight, only after verifying audience, moderation capability and advertiser agreements. Document approval, refund, expiration and takedown.

**Data model**: submission_id, studio_name, game_title, official_urls, ownership_attestation, review_status, sponsored (boolean), sponsor_disclosure, starts_at, expires_at. Avoid displaying contact emails publicly.

**Acceptance**: no paid placement without manual approval, disclosures visible in list and detail view, expired placements auto-unpublish or revert to organic, invalid links safely disabled.

## Track B — Gaming Deals / Affiliates
Build a voluntarily visited **Gaming Deals** page. List approved retailers and legitimate opt-in partner programs only. No claims of an affiliate partnership until accepted. Each deal includes game/product, retailer, price with currency and checked timestamp when available, official landing URL, expiration, and an adjacent **Affiliate link — we may earn a commission** label. Avoid implying prices are real-time when they are not. Never embed unapproved trackers or auto-redirect search results.

**Data model**: deal_id, title, merchant, official_url, partner_url, affiliate_approved, disclosure, verified_at, expires_at, visible; all outbound domains validated; redirect-to-untrusted-scheme blocked.

**Acceptance**: all displayed partner links are explicitly approved, disclosure adjacent, price/date shown appropriately, broken/expired offers hidden, no covert tracking or affiliate substitution on ordinary links.

## Track C — Support Retro Relay
Add a non-intrusive **Support Retro Relay** link in About/Settings and (optionally) the repository README. A real public donation/payment URL is required and must be user-owned and approved before it is embedded. GitHub Sponsors can be considered if eligible; other provider choices require user setup.

No payment information collected by the browser. Open the provider checkout in an intentionally clear page/tab; maintain the same free product regardless of payment.

**Acceptance**: missing provider URL means do not show a dead payment action; user can hide support prompt; no paywalls; no recurring charge without explicit provider consent; funding link comes only from the verified project owner.

## Implementation sequence
1. Product design and privacy/compliance review, including disclosures and licensing of artwork.
2. Add sponsor submission workflow and moderation.
3. Add opt-in affiliate deals page with verified offers.
4. Add support entry in About/Settings after the owner provides an approved payment URL.
5. Run tests: secure URL handling, absent links, sponsor disclosure, data storage, privacy, free features unchanged, separation from browsing profile.
6. Package and manually test on Windows; prepare next beta only after it passes.

## External dependencies
- Need the actual browser source files from the Windows workstation to implement and test UI; current public GitHub repository contains documentation and release notes, not the Python application source.
- Need legitimate sponsor agreements, affiliate approvals and an authorized support payment page.
- Income is not guaranteed. The project owner controls prices, links, publication and financial accounts.

## Legal/disclosure note
US FTC guidance requires clear, conspicuous disclosures for material connections. Confirm current program terms and applicable tax/privacy obligations before accepting funds.
