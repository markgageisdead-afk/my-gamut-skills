# San Antonio Cultural Event Lead Scout

## Purpose

Find and qualify San Antonio-area markets, pop-ups, festivals, fundraisers, and cultural events that may benefit from an experiential photo activation or sponsor-branded photo booth.

This skill produces a research-backed lead list and draft outreach. It does **not** send messages, create accounts, bypass access controls, or collect private contact information.

## Operating procedure

### 1. Define the search window

Ask for or infer:

- Target date range
- Preferred event radius from San Antonio
- Minimum expected attendance, if known
- Activation type: photo booth, roaming photographer, GIF booth, branded backdrop, or sponsor activation

Default to events occurring in the next 90 days within the greater San Antonio area.

### 2. Discover events

Search publicly available event pages and organizer calendars, prioritizing:

- Eventbrite
- San Antonio Current
- Visit San Antonio
- City, venue, university, nonprofit, and neighborhood calendars
- Public Instagram/Facebook pages when their event details are visible without login

Use combinations of these keywords:

- `pop-up market`
- `art vendor market`
- `gala`
- `charity run`
- `First Friday`
- `Second Saturday`
- `cultural festival`
- `chili cook-off`
- `Fiesta`
- `Quinceañera`
- `prom committee`
- `UTSA tailgate`
- `alumni event`

Do not treat search snippets as confirmed facts. Open the source page and record the source URL and the date it was checked.

### 3. Extract and normalize

For every candidate, capture:

| Field | Requirement |
|---|---|
| Event name | Required |
| Date and time | Required when published |
| Venue and neighborhood | Required when published |
| Organizer | Required when identifiable |
| Public contact | Email, phone, or contact-page URL; never infer private data |
| Event URL | Required |
| Source checked | Required |
| Vendors mentioned? | Yes / No / Unknown |
| Sponsors mentioned? | Yes / No / Unknown |
| Photo activation mentioned? | Yes / No / Unknown |
| Attendance or audience | Published estimate only |
| Notes | Relevant context and uncertainties |

Use ISO dates (`YYYY-MM-DD`) when the source provides enough information. Preserve the original date text in notes when it is ambiguous.

Deduplicate events by normalized event name + date + venue. Keep multiple source URLs when they corroborate the same event.

### 4. Qualify leads

Apply these tags:

- `[HIGH PRIORITY]` — public evidence of vendors or sponsors, no mention of a photo booth/photo activation, and the event date is not past.
- `[SPONSORSHIP FIT]` — sponsor packages, vendor tiers, or fundraising language is published.
- `[AUDIENCE FIT]` — strong fit for Fiesta-themed corporate parties, Quinceañeras, high-end high school prom committees, or UTSA tailgating/alumni groups.
- `[NEEDS VERIFICATION]` — date, organizer, venue, or contact details are incomplete or conflicting.
- `[LOW CONFIDENCE]` — only a listing snippet or unverified social post was found.

A lead can have multiple tags. Never claim that an event lacks a photo booth unless the checked event page or published sponsor/vendor materials support that conclusion; use “no activation found in the sources checked.”

Suggested score:

- +3 vendors explicitly listed
- +3 sponsors or sponsor packages explicitly listed
- +2 no photo activation found in checked sources
- +2 audience or event type is a target niche
- +1 published attendance above 100
- +1 event is within 90 days
- −2 contact or organizer is unavailable
- −2 date or venue is unverified

Interpretation: 7+ = high priority; 4–6 = research/outreach candidate; 0–3 = monitor.

### 5. Recommend the sponsorship angle

For qualified leads, explain how the organizer could offer a local business a sponsor-branded activation. Keep claims proportional to the evidence. Example positioning:

> A local business could sponsor the photo activation. The sponsor receives logo placement on digital prints and shared content, while the event receives a crowd-friendly activation without carrying the full cost.

Do not promise guaranteed attendance, impressions, sponsor revenue, or free service unless those terms are actually approved by the photo-activation provider.

### 6. Draft, do not send, outreach

Use the public organizer name and confirmed event details only:

> Hey [Organizer Name], noticed you are putting together the [Event Name] at [Venue]. Large crowds love capturing these moments. If you have sponsors lined up, we can brand every photo with their logo—helping you secure higher sponsor tiers while keeping your attendees buzzing. Do you have a photo activation locked in for [Date] yet?

Add one specific observation from the source page and a clear opt-out or low-pressure next step when appropriate. Do not mass-message, impersonate an organizer, or contact private individuals without a relevant public role.

## Output format

Return:

1. A short summary of the search window, geography, sources, and limitations.
2. A table of all discovered events with the required extraction fields.
3. A ranked shortlist with tags, score, evidence, and recommended angle.
4. Draft outreach messages for only the top qualified leads.
5. A follow-up checklist showing what must be verified before contact.

Always include source URLs and the “checked on” date for every lead.

## Quality and safety rules

- Use only publicly available information and respect site terms, robots directives, rate limits, and platform access controls.
- Do not scrape behind logins, evade bot protections, or collect sensitive personal data.
- Treat email addresses and phone numbers as business contact data only when the source presents them for event/business contact.
- Distinguish confirmed facts, reasonable inferences, and unknowns.
- Never fabricate an organizer, contact, venue, sponsor, attendance figure, or event date.
- If web access is unavailable, provide a research plan and clearly label the results as incomplete.
