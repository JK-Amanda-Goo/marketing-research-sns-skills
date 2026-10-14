---
name: marketing-research-instagram-vid
description: Researches Instagram Reels to find hook and format best practices a brand can copy tomorrow, then delivers a compact 3-tab Google Sheet (Setup & Method, Best Practices, Log Highlights) with fill-in-the-blank templates and clickable source links. It first asks whether going viral or building industry credibility matters more and tailors the sample to that. Use when someone wants Reels hook research, Instagram video best practices, what video formats work for their brand, competitor Reels analysis, or content ideas grounded in real examples. Not for carousels (use marketing-research-instagram-carousel), TikTok (use marketing-research-tiktok-vid), ad creative testing, or posting and scheduling.
---

# Marketing Research: Instagram Reels

Find what actually works in Instagram Reels for this user's product and audience, and hand back a short playbook they can film from.

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

Use Instagram search and the Reels tab on profiles. Combine: topic keywords, format words ("brand list", "outfit of the day", "how I", "things I wish I knew"), the user's reference accounts, and accounts that keep appearing. Aim to look at 25 to 40 Reels from at least 15 accounts.

**Mix the formats on purpose.** Do not research only UGC. Cover creator-to-camera, list or roundup, tutorial or how-to, interview or conversation, behind the scenes, text-on-screen with trending audio, founder or expert talk, and faceless. The point is to find formats the user has not thought of that fit what they can produce (intake answer 5).

## Step 3: Measure

For each Reel record: account, followers, link, date, views, likes, comments.
- **x median** = this Reel's views divided by the median views of that account's other recent Reels (10 to 14 of them). It shows whether the Reel beat the account's normal, so a 40K-view Reel on a 300K-view account does not look like a win.
- Accounts under about 10K followers: keep, but flag the small-account bias.

## Step 4: Capture the hook

- If a transcript or captions are available, quote the **actual spoken hook** (first sentence or two). Label it `Spoken`.
- If not, use the on-screen text in the first seconds plus the caption. Label it `On-screen`. Never present on-screen text as a spoken line.
- Also note the format, the CTA (comment keyword, save, follow, link in bio, none), and the maker type (creator, brand, expert).

## Step 5: Synthesize

Group Reels into patterns by hook type and format. Apply the evidence rule, map each pattern to an intake problem statement, filter and order by the user's priority, and write a fill-in-the-blank hook template for each Best practice (`[Number] [things] that [outcome] without [pain]`, with a real example from the log).

Known limits to state in the sheet: saves and shares are not public; search results favour hits (survivor bias); x median is rough; instagram search is personalised; hooks without transcripts are on-screen only.

## Evidence rule

- **Best practice** = seen in 3 or more Reels from 2 or more accounts.
- **Hypothesis** = fewer than that. Say so plainly.
- **Do not copy** = spreads but got little engagement, or conflicts with the user's brand.
- **Gap** = a problem statement with no evidence found. Say so instead of filling it.

Never invent a number, a link or a quote. If a value could not be read, write `n/a`.

## Output: one Google Sheet, always these 3 tabs

Compact beats complete. A reader should know what to do after five minutes.

**Tab 1: Setup & Method** (label in column A, text in column B)
Goal, Product and audience, Priority (viral or credibility, and what that changed), Problem statements, Method (4 to 6 numbered steps of what was actually done), Selection criteria, Metrics used, Sample (how many Reels from how many accounts, date researched), Evidence rule, Limits (what this research cannot tell you).

**Tab 2: Best Practices** (max 10 rows, plus max 3 "Do not copy" rows)
Columns: `#` | `Pattern` | `Status` | `Problem it serves` | `What we saw` (numbers) | `Your version` (fill-in-the-blank hook and structure) | `Examples` (log row numbers, clickable links) | `Caution`.
Order: Best practice, then Hypothesis, then Do not copy. Colour the status cell: green, yellow, red. Add a Gap row for any problem statement without evidence.

**Tab 3: Log Highlights** (15 to 20 rows, only the Reels that back a best practice or a do-not-copy)
Columns: `#` | `Account` | `Followers` | `Reel link` | `Date` | `Views` | `Likes` | `Comments` | `x median` | `Hook (spoken or on-screen)` | `Format` | `CTA` | `Takeaway` | `Supports #`.
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
