---
name: sa-event-scout
description: Find and qualify San Antonio-area markets, festivals, fundraisers, and cultural events for sponsor-branded photo activations and photo booths.
---

# San Antonio Cultural Event Lead Scout

## Purpose

Find and qualify San Antonio-area markets, pop-ups, festivals, fundraisers, and cultural events that may benefit from an experiential photo activation or sponsor-branded photo booth.

This skill produces a research-backed lead list and draft outreach. It does not send messages, create accounts, bypass access controls, or collect private contact information.

## Operating procedure

### 1. Define the search window

Ask for or infer:

- Target date range
- Preferred event radius from San Antonio
- Minimum expected attendance, if known
- Activation type: photo booth, roaming photographer, GIF booth, branded backdrop, or sponsor activation

Default to events occurring in the next 90 days within the greater San Antonio area.

### 2. Discover events

Search publicly available event pages and organizer calendars, prioritizing Eventbrite, San Antonio Current, Visit San Antonio, city and venue calendars, universities, nonprofits, neighborhood calendars, and public social pages visible without login.

Useful search terms include:

- pop-up market
- art vendor market
- gala
- charity run
- First Friday
- Second Saturday
- cultural festival
- chili cook-off
- Fiesta
- Quinceañera
- prom committee
- UTSA tailgate
- alumni event

Do not treat search snippets as confirmed facts. Open the source page and record the source URL and the date checked.

### 3. Extract and normalize

For each candidate, capture:

- Event name
- Date and time
- Venue and neighborhood
- Organizer
- Public business contact, if published
- Event URL and source URL
- Whether vendors, sponsors, or a photo activation are mentioned
- Published attendance or audience information
- Relevant notes and uncertainties

Use ISO dates (`YYYY-MM-DD`) when the source provides enough information. Preserve the original date text when it is ambiguous. Deduplicate by normalized event name, date, and venue.

### 4. Qualify leads

Apply one or more of these tags:

- `[HIGH PRIORITY]` — public evidence of vendors or sponsors, no photo activation found in checked sources, and the event date is not past.
- `[SPONSORSHIP FIT]` — sponsor packages, vendor tiers, or fundraising language is published.
- `[AUDIENCE FIT]` — strong fit for corporate parties, Quinceañeras, prom committees, UTSA tailgates, or alumni groups.
- `[NEEDS VERIFICATION]` — date, organizer, venue, or contact details are incomplete or conflicting.
- `[LOW CONFIDENCE]` — only a listing snippet or unverified social post was found.

Suggested score:

- +3 vendors explicitly listed
- +3 sponsors or sponsor packages explicitly listed
- +2 no photo activation found in checked sources
- +2 audience or event type is a target niche
- +1 published attendance above 100
- +1 event is within 90 days
- −2 contact or organizer is unavailable
- −2 date or venue is unverified

Interpretation: 7+ is high priority; 4–6 is a research/outreach candidate; 0–3 is monitor.

Never claim that an event lacks a photo booth unless the checked event page or published sponsor/vendor materials support that conclusion. Use “no activation found in checked sources” when appropriate.

### 5. Recommend the sponsorship angle

For qualified leads, explain how an organizer could offer a local business a sponsor-branded activation. Keep claims proportional to the evidence. Do not promise guaranteed attendance, impressions, sponsor revenue, or free service unless those terms are approved by the photo-activation provider.

### 6. Draft, do not send, outreach

Use only the public organizer name and confirmed event details. Include one specific observation from the source page and a low-pressure next step. Do not mass-message, impersonate an organizer, or contact private individuals with personal information.

## Output format

Return:

1. A short summary of the search window, geography, sources, and limitations.
2. A table of all discovered events with the extraction fields above.
3. A ranked shortlist with tags, score, evidence, and recommended angle.
4. Draft outreach messages for only the top qualified leads.
5. A follow-up checklist showing what must be verified before contact.

Always include source URLs and the date checked for every lead.

## Quality and safety rules

- Use only publicly available information and respect site terms, robots directives, rate limits, and platform access controls.
- Do not scrape behind logins, evade bot protections, or collect sensitive personal data.
- Treat email addresses and phone numbers as business contact data only when the source presents them for event or business contact.
- Distinguish confirmed facts, reasonable inferences, and unknowns.
- Never fabricate an organizer, contact, venue, sponsor, attendance figure, or event date.
- If web access is unavailable, provide a research plan and clearly label results as incomplete.
