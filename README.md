# Northwestern Medicine Downtown Transfer Hub — independent concept

A responsive, dependency-free demonstration of a transfer coordination command center. **Not an official Northwestern Medicine system, not affiliated with or endorsed by Northwestern Medicine, and not connected to Epic. All operational data is fictional. Do not enter real patient information.**

## Preview

- Dashboard: searchable queue, intersecting priority/stage filters, escalation view, pagination, request detail, workflow, ownership, and in-session demo actions.
- Intake: controlled sample values create fictional requests. No patient identifiers or clinical free-text fields.
- Capacity: explicitly illustrative capacity by level of care.
- Communications: session activity history; no messages are sent.
- Analytics: values calculated from the current demo queue.
- Referring clinicians: separate `#referring` page with official transfer contact link.
- Integration plan: `#integration` describes the production boundary.

## Run locally

Node.js 20 or newer. No packages to install.

```sh
npm start
# Open http://127.0.0.1:4173
npm test
```

The source is static HTML, CSS, and JavaScript, so GitHub Pages can serve it directly from the main branch root. Hash navigation supports subdirectory hosting without rewrites. Fonts load from Google Fonts with local fallbacks.

## GitHub Pages

In Settings → Pages, choose **Deploy from a branch**, then **main / (root)**. The `.nojekyll` file enables direct static serving. All published data is fictional. The public static preview has no staff access controls and is not a clinical application.

## State and limits

Changes exist in browser memory only and reset on refresh. Wait times are a fixed illustrative snapshot, not live clocks. Demo stage advancement does not perform clinical acceptance or change any hospital system. Capacity values are separate sample fixtures. The source does not include credentials or analytics trackers. No localStorage, cookies, patient records, external API calls, or live messages are used.

## Production integration

Deploying a real internal tool requires an organization-approved backend, single sign-on, server-enforced roles, audit logging, validated source timestamps, stale-feed handling, secure configuration, and approved interfaces to Epic, bed management, and telephony. Epic remains authoritative for clinical documentation, acceptance, bed assignments, and transport events. Do not invent or expose Epic endpoints in the static client. Browser-only UI restrictions are not security controls.

## Official sources

Reviewed October 29, 2026:

- [NM transfer contact information](https://www.nm.org/conditions-and-care-areas/pulmonary/critical-care-medicine)
- [Epic Transfer Center FAQ, June 2023](https://physicianforum.nm.org/uploads/1/1/9/4/119404942/transfer_center_faq_final_physician_forum_6.13.2023.pdf)

The older FAQ is background for the concept, not proof of a current approved integration contract. Northwestern Medicine names identify the proposed destination; this repository contains no official logo assets.
