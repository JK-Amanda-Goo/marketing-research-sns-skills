---
name: marketing-research-competitors
description: Researches competitors and substitutes for an early-stage product to support positioning, pricing, first-channel and product-market-fit decisions, then delivers a compact 4-tab Google Sheet (Setup & Method, Best Practices, Log Highlights, Customer Voice) with copy/avoid/white-space moves, one profile row per competitor and sourced customer quotes, all with clickable links. It first asks which decision the research should support. Use when someone wants competitor analysis, a competitive landscape, positioning research, pricing benchmarks, "who else does this", customer complaints about alternatives, or white-space opportunities for a new product. Not for social-media content analysis (use marketing-research-instagram-vid, -instagram-carousel or -tiktok-vid), financial modelling, SWOT or strategy decks, or contacting competitors.
---

# Marketing Research: Competitors

Find where this product can stand out and what to do first, using what competitors say, charge, do and what their customers say about them.

The deliverable is deliberately small: a method record, a short list of moves, one row per competitor, and a page of real customer quotes. The useful output is not "what competitors do" but "so where do we stand, and what do we do next".

## Step 1: Intake (ask once, in one message)

Ask these in a single short message, one line each. Skip anything the conversation already answers. If the user says "you decide", pick a sensible default and name it in the sheet.

1. **Product, stage, audience**: one line for the product; stage (idea / MVP / pre-launch / launched); who it is for.
2. **The decision this research must support**: positioning, pricing, first marketing channel, or feature priority. Pick the most urgent one. It sets the weight of the work (see below).
3. **Known competitors or references**: names or links, if any.
4. **Market and language**: country or city, language.

How the decision changes the work:
- **Positioning**: spend most effort on messaging, target customer and customer quotes.
- **Pricing**: spend most effort on price pages, plans, free tiers and what customers say about value.
- **First channel**: spend most effort on where competitors acquire customers and with what offer.
- **Feature priority**: spend most effort on product gaps and customer complaints.

## Step 2: Build the competitor set (5 to 8, no more)

- 3 to 4 **direct** competitors (same customer, same job).
- 2 to 3 **substitutes** (what people do instead: spreadsheets, offline habits, a general tool, doing nothing).
- 1 to 2 **adjacent / inspiration** (a different market with a model worth borrowing).

Find them with web search, app-store search, Reddit threads ("alternatives to", "what do you use for") and the user's references. Show the set to the user in one line each and get a quick yes before going deep.

## Step 3: Research each competitor

For each one, read the public pages and record:
- **Positioning**: the one-line promise and the target customer, in their words (homepage, store listing, bio).
- **Product**: core features, onboarding or first-run if visible, one clear gap.
- **Pricing**: plans, price, free tier, business model. `n/a` if hidden.
- **Acquisition**: main channels and the message or offer used (social, SEO, ads library, partners, influencers). If a social channel is worth a deeper look, name the account so the user can run the Instagram or TikTok skills on it.
- **Traction signals**: store rating and review count, traffic or download estimates, funding, founding year, team size. Always label estimates as `est.`.

## Step 4: Collect the customer voice

This is the most valuable part for product-market fit. Pull real, public customer language from app-store reviews, Reddit, G2 / Trustpilot, Product Hunt and video comments. For each competitor read roughly 20 to 40 recent items, and keep the 3 to 5 quotes that best show:
- what people **praise** (the job it does well),
- what they **complain about** (the unmet need),
- what they **wish existed** or why they **switched / left**.

Quote exactly and keep each quote short. Reviews skew toward complaints, so also record how many items you read and say so in Limits.

## Step 5: Synthesize

Turn everything into at most 10 moves, each tied to the decision from intake:
- **Copy**: something several competitors do that works, and how to do it for this product.
- **Avoid**: something that fails or that customers complain about.
- **White space**: a need many customers voice that few competitors serve. Offer 1 to 3.

Each move ends with a concrete next action ("Test this headline", "Price at X with a free trial", "Build Y first").

## Evidence rule

- **Best practice** = seen at 3 or more competitors, or in customer quotes from 3 or more different sources.
- **Hypothesis** = fewer than that. Say so plainly.
- **Gap** = a question the decision needs that no evidence answers. Say so instead of filling it.

Never invent a number, a link or a quote. If a value could not be read, write `n/a`.

## Output: one Google Sheet, always these 4 tabs

Compact beats complete. A reader should know what to do after five minutes.

**Tab 1: Setup & Method** (label in column A, text in column B)
Goal, Product and audience, Decision to support (and what that changed), Method (4 to 6 numbered steps actually done), Competitor set and why, Sample (competitors, review items read, date researched), Evidence rule, Limits.

**Tab 2: Best Practices** (max 10 rows)
Columns: `#` | `Move` | `Type` (Copy / Avoid / White space) | `Status` (Best practice / Hypothesis) | `What we saw` (with numbers) | `Do this next` | `Evidence` (competitor names, Customer Voice row numbers, clickable links) | `Caution`.
Order: Best practice first, then Hypothesis. Colour the status cell: green, yellow. Add a Gap row for any open question.

**Tab 3: Log Highlights** (one row per competitor, 5 to 8 rows)
Columns: `#` | `Competitor` | `Type` (Direct / Substitute / Adjacent) | `Link` | `Positioning (their words)` | `Target customer` | `Price and model` | `Main channels` | `Top strength` | `Top gap` | `Traction (est.)` | `Supports #`.
The link column must be a clickable hyperlink to the competitor's page. `Supports #` points to the Best Practices row.

**Tab 4: Customer Voice** (15 to 30 rows)
Columns: `#` | `Competitor` | `Source` (App Store / Reddit / G2 / ...) | `Link` | `Date` | `Quote` | `Theme` (Praise / Complaint / Wish / Switched) | `Job or need behind it` | `Supports #`.
The link column must be a clickable hyperlink to the original review or thread. Keep quotes short and verbatim.

Deliver the sheet:
1. If a Google Drive connector is available, create a native Google Sheet. A method that works: write a SpreadsheetML 2003 XML workbook (4 `Worksheet` elements) and upload it with `contentMimeType: application/vnd.ms-excel`; Drive converts it to a multi-tab Sheet. Use `ss:HRef` on a cell for clickable links and `ss:StyleID` for fills. Read the file back and check all 4 tabs, the links and the numbers before reporting.
2. Otherwise write an `.xlsx` (for example with openpyxl, with real hyperlinks) and tell the user to upload it to Drive.

Keep the sheet private; do not share it unless asked. Write the sheet in English unless the user asks otherwise; chat can be in the user's language.

Finish with a short chat summary: the link, the top 3 moves, the biggest white space, and the main limit. Do not paste the sheet into chat.

## Limits to state in the sheet

- Traffic, download and funding figures are estimates.
- Reviews skew toward complaints and toward people who feel strongly.
- Only public information is used; no logins, no private data, and no contact with competitors.
- A small competitor set (5 to 8) shows patterns, not the whole market.

## Ground rules

- Public content only. Record links; do not download files.
- Use the user's own browser session through the browser tool. Never type passwords or work around logins, paywalls, captchas or blocks. If a site blocks you, stop, say so in Limits, and continue by hand.
- Keep tool output short; long outputs get truncated.
- Give the user a one-line status every few steps during long collection.
