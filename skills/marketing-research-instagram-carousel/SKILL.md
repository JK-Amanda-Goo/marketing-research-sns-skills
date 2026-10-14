---
name: marketing-research-instagram-carousel
description: Researches Instagram carousels to find cover, slide-structure and caption-CTA best practices a brand can copy tomorrow, then delivers a compact 3-tab Google Sheet (Setup & Method, Best Practices, Log Highlights) with slide-by-slide templates and clickable source links. It first asks whether going viral or building industry credibility matters more and tailors the sample to that. Use when someone wants carousel research, Instagram carousel best practices, what slide formats get saved, or carousel ideas grounded in real examples. Not for Reels (use marketing-research-instagram-vid), TikTok (use marketing-research-tiktok-vid), graphic design, or posting and scheduling.
---

# Marketing Research: Instagram Carousels

Find what actually works in Instagram carousels for this user's product and audience, and hand back slide-by-slide templates they can build from.

The deliverable is deliberately small: a one-tab setup and method record, a short list of best practices the user can apply immediately, and a log of the highlighted examples with numbers and clickable links. People want something they can use today, not a data dump.

## Step 1: Intake (ask once, in one message)

Ask these in a single short message and let the user answer in a line each. Skip anything the conversation already answers. If the user says "you decide" on something, pick a sensible default and name it in the sheet.

1. **Product and audience**: what is it, and who is it for? One line each.
2. **Primary priority: viral or credibility?** Which matters more right now: going viral (reach, new eyes) or building credibility in your industry (trust with a specific niche)? Pick one as primary. "Mostly X, a little Y" is fine.
3. **Audience problems**: 3 to 7 short statements of the problems your content should speak to. If they have none, propose 3 to 5 from answer 1 and get a yes.
4. **Goal action**: what should a viewer do after watching (follow, join a waitlist, DM, buy, visit)?
5. **What you can realistically produce**: face on camera, voiceover only, no-face, designer-made, UGC-style; time per piece.
6. **Market and references**: country or city, language, and any accounts or competitors they already know.

How priority changes the work:
- **Viral**: pick samples by reach relative to account size, score patterns by hook strength and share/save potential, and allow adjacent formats from other niches if they transfer.
- **Credibility**: pick samples from recognised voices in the niche, weight proof elements (expertise, real examples, behind the scenes) and comment quality, and drop pure trend-bait even when it got reach.

## Step 2: Discover

Use Instagram search and profile grids. Combine: topic keywords, format words ("capsule", "guide", "checklist", "save this"), "comment [word] for" CTAs, the user's reference accounts, and accounts that keep appearing. Aim to look at 20 to 30 carousels from at least 12 accounts. Carousels only; skip single images and Reels.

Mix the maker types (creator, brand, expert) and the formats (guide, list, before/after, story, template or series). Check what the user can produce (intake answer 5) and keep options they can actually make.

## Step 3: Measure

For each carousel record: account, followers, link, date, likes, comments, slide count.
- **Comments per like** shows conversation density. Comment counts include replies and keyword-CTA spam, so read them with care.
- **x median (likes)** = this carousel's likes divided by the median likes of the account's other visible carousels. It is rough, so say so.
- Accounts under about 10K followers: keep, but flag the small-account bias.

## Step 4: Capture the structure

Read the **cover (slide 1)**, the **last slide**, and as many middle slides as load. Record cover text, a one-line structure ("cover / 6 tips / recap / CTA"), and the caption CTA. Mark capture level (`Full`, `Partial`, `Caption only`) so the reader knows how much was seen.

## Step 5: Synthesize

Group carousels by cover type and slide structure. Apply the evidence rule, map each pattern to an intake problem statement, filter and order by the user's priority. For each Best practice write the `Your version` as a slide-by-slide template (Slide 1: cover line pattern; Slides 2 to N: what each carries; last slide: CTA wording) plus a caption and CTA template, with a real example from the log.

Known limits to state in the sheet: saves and shares are not public and carousels often win on saves, so likes and comments understate them; search results favour hits; x median is rough; some slides may not load; Instagram search is personalised.

## Evidence rule

- **Best practice** = seen in 3 or more carousels from 2 or more accounts.
- **Hypothesis** = fewer than that. Say so plainly.
- **Do not copy** = spreads but got little engagement, or conflicts with the user's brand.
- **Gap** = a problem statement with no evidence found. Say so instead of filling it.

Never invent a number, a link or a quote. If a value could not be read, write `n/a`.

## Output: one Google Sheet, always these 3 tabs

Compact beats complete. A reader should know what to do after five minutes.

**Tab 1: Setup & Method** (label in column A, text in column B)
Goal, Product and audience, Priority (viral or credibility, and what that changed), Problem statements, Method (4 to 6 numbered steps of what was actually done), Selection criteria, Metrics used, Sample (how many carousels from how many accounts, date researched), Evidence rule, Limits (what this research cannot tell you).

**Tab 2: Best Practices** (max 10 rows, plus max 3 "Do not copy" rows)
Columns: `#` | `Pattern` | `Status` | `Problem it serves` | `What we saw` (numbers) | `Your version` (slide-by-slide plus caption and CTA) | `Examples` (log row numbers, clickable links) | `Caution`.
Order: Best practice, then Hypothesis, then Do not copy. Colour the status cell: green, yellow, red. Add a Gap row for any problem statement without evidence.

**Tab 3: Log Highlights** (15 to 20 rows, only the carousels that back a best practice or a do-not-copy)
Columns: `#` | `Account` | `Followers` | `Carousel link` | `Date` | `Likes` | `Comments` | `Comments per like` | `x median (likes)` | `Slides` | `Cover text` | `Slide structure` | `CTA` | `Takeaway` | `Supports #`.
The link column must be a clickable hyperlink to the original post. Every row carries its basic numbers. Include a `Supports #` column pointing to the Best Practices row.

Deliver the sheet:
1. If a Google Drive connector is available, create a native Google Sheet. A method that works: write a SpreadsheetML 2003 XML workbook (3 `Worksheet` elements) and upload it with `contentMimeType: application/vnd.ms-excel`; Drive converts it to a multi-tab Sheet. Use `ss:HRef` on a cell for clickable links, `ss:Formula` in R1C1 style for ratios, and `ss:StyleID` for fills. Read the file back and check all 3 tabs, the links and the computed numbers before reporting.
2. Otherwise write an `.xlsx` (for example with openpyxl, with real hyperlinks) and tell the user to upload it to Drive.

Keep the sheet private; do not share it unless asked. Write the sheet in English unless the user asks otherwise; chat can be in the user's language.

Finish with a short chat summary: the link, the top 3 best practices, and the main limit. Do not paste the sheet into chat.

## Ground rules

- Public content only. Record links, never download videos or images.
- Use the user's own browser session through the browser tool. Never type passwords or work around logins, captchas or blocks. If the site blocks you, stop, say so in Limits, and continue by hand.
- Keep tool output short; long outputs get truncated.
- Give the user a one-line status every few steps during long collection.
