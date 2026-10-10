# Follow-ups

This file records anything deferred mid-build, one numbered item per entry. New items are appended as they come up. When an item closes, a status block is appended above the original entry rather than deleting or rewriting it; if the original entry's framing turns out to have been wrong, that is said explicitly in the status block. A status block that closes only part of an item — a lettered sub-item, or a single paragraph or ruling inside it — sits directly below the paragraph it closes instead. A lettered ruling that settles part of an open item without closing it sits indented directly below the entry, with no Status line. A status line that closes, parks or records a numbered item opens in one fixed form: `**Status (YYYY-MM-DD): open | closed | closed, parked | ruled at filing | record — ruling XX.**` When an item's status changes, the new line goes above the earlier ones, which stay as history, so the first status line above any number is the authority. Every close-out logs each carry the item listed as applied, declined or re-filed.

**Status (2026-10-10): record — ruling A.** Not a task; the entry records two standing policies for this guide, ruled by the owner in chat on 2026-10-08 and 2026-10-10, before any content page landed.

1. **Standing policies ruled before the build.** (a) No AI tool, platform or brand name appears anywhere in the guide — body prose, Go deeper links, glossary, worksheets, metadata — with two carve-outs: the project's own name and hub link, and links to the project's own compliance checker. (b) Figures set by law, regulation or an agency live only on the one figures page, never in body prose; the topic was chosen so that page stays short, ideally empty.

**Status (2026-10-10): ruled at filing — ruling B.**

2. **Step list.** Six steps of the process, in order, slugs as named in CLAUDE.md under Structure: Decide what to use it for; Understand how it answers; Choose what you share; Ask it well; Check what it tells you; Act, record and review. The last links back to the first.

**Status (2026-10-10): ruled at filing — ruling C.**

3. **Knowledge areas.** Six areas, in order: How language models answer; Privacy and your data; Primary sources; Numbers and assumptions; Scams and impersonation; Information versus advice. Money-topic areas (budgeting, investing, tax) are out of scope; those belong to the Financial Planning Guide and are linked, not repeated.

**Status (2026-10-10): ruled at filing — ruling D.**

4. **Tools.** The figures page plus one checklist, Checking an answer, using the template's checklist variant. No worksheets at launch. The figures page ships with one H2 per area and no rows; the figures audit found no figure set by law, regulation or an agency that any planned page turns on.

**Status (2026-10-10): ruled at filing — ruling E.**

5. **Process name and area label.** The process is The Ask-Then-Check Loop; the knowledge areas are labelled Foundations. Both chosen after the step and area lists were settled.

**Status (2026-10-10): ruled at filing — ruling F.**

6. **"For practitioners" Callout re-aimed.** The step-skeleton instruction for the Callout is reworded in this repo's CLAUDE.md only: what you would tell a client doing this step on their own, and what to note in their file. Heading, position and length are unchanged; guide-template is not changed.

7. **Template build-out checklist, carried from the deleted CLAUDE.md section.** Still to edit: README.md (title, description, repository URL); app/layout.jsx (REPO_URL check); content/_meta.js, content/process/_meta.js, content/domains/_meta.js, content/tools/_meta.js (entries as each page lands); the four landing pages (introduction, process, domains, tools); content/about/index.mdx (author line, disclaimer sentence, corrections URL, license links); content/glossary/index.mdx (drop the example term with the first real term); content/process/example-step and content/domains/example-area (delete after the first real step and area land); content/tools/this-years-figures/index.mdx (six H2s); LICENSE copyright line. Close when the token grep in CLAUDE.md's former line 4 returns zero hits.

Next free ruling letter: G.
