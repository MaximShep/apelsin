# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **strategic research project** analyzing X5 Group's **Apelsin payment card** — a debit card co-branded with Alfa-Bank targeting Russian youth (18–25). The goal is to develop recommendations for increasing card adoption and usage among young adults.

The main case brief is in `X5.md`. All research is in `research/`.

## Research Structure & Reading Order

The `research/` files are numbered to indicate logical reading order:

- `00_insights.md` — Synthesis of all findings; three strategic hypotheses (start here for orientation)
- `01_youth_behavior.md` — Target audience analysis (18–25 banking preferences)
- `02_apelsin_product.md` — Current product mechanics, barriers, and UX analysis
- `03_competitors_russia.md` — Russian competitors: T-Bank, Yandex, Magnit, Samokat
- `04_global_cases.md` — Global benchmarks: Starbucks, Revolut, Monzo, Amazon Prime
- `05_habit_formation.md` — Behavioral economics and habit-formation psychology
- `06_russian_superapps.md` — Marketplace-fintech strategies: Ozon Bank, WB Bank, Yandex Pay
- `07_global_loyalty_debit.md` — Retail loyalty + debit card hybrids: Tesco, Target, Kroger

`00_insights.md` is the synthesis point — its conclusions draw on evidence from files `01`–`07`.

## Key Problem & Strategic Directions

**The core problem:** Apelsin's 7% cashback fails to drive behavioral change because:
- Young people already have 2–3 cards; inertia beats rational arguments
- Cashback accumulates slowly (no immediate feedback)
- Complex mechanics (6% card + 1% club + 5% subscription tiers)
- Card is useless outside X5 stores (only 1% cashback elsewhere)

**Three strategic directions in `00_insights.md`:**
1. **Visible Loss Now** — Show "Price with Apelsin: 89р / Without: 99р" at shelf (Tesco Clubcard model)
2. **Capture at Life Transitions** — Target when habits aren't yet formed (students, movers, first job)
3. **Viral Through Ritual** — Referral mechanics embedded in natural group shopping behavior

## Web Research Permissions

Configured in `.claude/settings.local.json` to allow fetching from:
- `vc.ru` — Russian tech/business media
- `banki.ru` — Russian banking product database
- `finance.ozon.ru` — Ozon financial products

Use subagents with Haiku 4.6 for any exploration or research. If a task needs 3+ files or multi-file analysis, spawn a subagent and return only summarized insights. For thinking or coding use Sonnet