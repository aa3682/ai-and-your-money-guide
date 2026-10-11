# AI and Your Money Guide

An open, public reference on using AI on your own money without being misled, from deciding what to ask it to checking what it tells you before you act.

- Live site: https://ai-and-your-money-guide.vercel.app
- Part of the [AlignFlow](https://alignflow-hub.vercel.app) guides

Built on Nextra 4 from the AlignFlow guide template, with a process-first structure, one reference page for regulated figures, and a `CLAUDE.md` that sets the writing conventions.

## What this is

A free guide for anyone who manages their own money and uses an AI assistant for questions about it, and for the adviser or planner whose clients do. It is educational material, not financial, tax, legal, or investment advice.

The site has six sections: introduction, process, Foundations, tools, glossary, about.

**The Ask-Then-Check Loop** (process), six steps in order:

1. Decide what to use it for
2. Understand how it answers
3. Choose what you share
4. Ask it well
5. Check what it tells you
6. Act, record and review

**Foundations** (domains), the six bodies of knowledge the steps draw on:

- How language models answer
- Privacy and your data
- Primary sources
- Numbers and assumptions
- Scams and impersonation
- Information versus advice

**Tools:** This year's figures (the only page that prints a limit, rate, threshold or deadline set by law or regulation, each row dated and sourced) and Checking an answer (a checklist).

Pages are added one at a time. `FOLLOWUPS.md` records what is open and every ruling made on the repo.

## Writing conventions

`CLAUDE.md` is the source of truth. The rules that shape every page:

- No AI model, platform, or brand names anywhere in the guide, and nothing commercial linked from it.
- All prose is original. Claims that need support cite a public primary source.
- Regulated figures never appear in body prose; they live on This year's figures.
- No personal data and no real client examples.
- Slate theme, dark mode only, no theme switch.

## Corrections

If you find an error, a broken link, or a figure that is out of date, open an [issue](https://github.com/aa3682/ai-and-your-money-guide/issues). Say which page and which line, and if you can, link the source that shows the correct fact.

## Author

Written by someone with more than fifteen years of hands-on experience inside wealth management and investment advisory, working from public primary sources. The guide is published under the AlignFlow project name.

## Stack

- [Nextra](https://nextra.site) 4 with `nextra-theme-docs`, restyled with a slate theme (dark only) in `app/globals.css`
- A slate code-highlighting theme in `code-theme.mjs`, passed to Nextra in `next.config.mjs`
- [Outfit](https://github.com/Outfitio/Outfit-Fonts), self-hosted from `fonts/` with `next/font/local`
- Next.js App Router
- MDX content in `content/`
- [Pagefind](https://pagefind.app) search index generated at build time
- [Playwright](https://playwright.dev) (dev only), for `pnpm theme-audit`
- pnpm as the only package manager

## Run locally

Requires Node.js 24 (`engines` and `.nvmrc` both pin it; Vercel reads `engines`) and [pnpm](https://pnpm.io).

```sh
pnpm install
pnpm dev
```

Then open http://localhost:3000.

## Build

```sh
pnpm build
pnpm start
```

`pnpm build` also generates the search index (Pagefind) into `public/_pagefind`.

On Vercel, `VERCEL_DEEP_CLONE=true` is set for Production and Preview. Without it Vercel clones the repository shallowly and Nextra warns "repository is shallow cloned" during the build.

`pnpm theme-audit [url]` re-checks the theme in a running build (`pnpm start`, default http://localhost:3000): dark mode forced, no theme switch, no neutral greys, text contrast and focus rings, on every sidebar page at 1280px and 390px. Run it after a Nextra upgrade or any colour change. The first run on a new machine needs `pnpm exec playwright install chromium`.

`pnpm wordcount <path>` counts the body prose of a content page, following the word-count rules in `CLAUDE.md`.

## License

The prose in `content/` is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The code is licensed under MIT (see `LICENSE`). The Outfit font in `fonts/` is licensed under the SIL Open Font License 1.1 (see `fonts/OFL.txt`).
