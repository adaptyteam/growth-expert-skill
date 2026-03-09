# iOS Monetization Expert — Claude Code Skill

A Claude Code skill that turns Claude into an expert iOS subscription monetization advisor. It gives direct, benchmarked advice grounded in real data from Adapty's State of In-App Subscriptions 2026 report ($3B revenue, 16,000+ apps).

## What It Does

When you ask monetization questions in Claude Code, this skill automatically activates and provides:

- **Instant benchmarking** — Compare your metrics (LTV, conversion, retention, churn) against industry data
- **Pricing guidance** — Region-specific pricing benchmarks across weekly, monthly, and annual plans
- **Trial strategy** — Whether to use free trials based on your category and plan type
- **Growth advice** — Which markets to target, when to raise prices, how to reduce churn
- **Direct answers** — No fluff, just what the data says and what you should do next

## Example Questions

- "How should I price my Health & Fitness app?"
- "How many free trial days should I offer?"
- "Should I add a weekly plan?"
- "Should I use a free trial or a direct paywall?"
- "Which countries should I target for the best LTV?"
- "What's a good install-to-paid conversion rate?"
- "How do I reduce churn on my annual plan?"

## Installation

1. Clone the repository:

```bash
git clone https://github.com/adaptyteam/growth-expert-skill.git
```

2. Create the Claude skills directory if it does not exist:

```bash
mkdir -p ~/.claude/skills
```

3. Copy the skill into your Claude skills folder:

```bash
cp -R growth-expert-skill/ios-monetization-expert ~/.claude/skills/
```

4. Restart Claude Code.

## Data Coverage

The skill includes benchmarks for:

| Area | Details |
|------|---------|
| **LTV** | 12-month LTV by category, country, and install LTV |
| **Pricing** | Regional pricing, pricing index (US baseline), price tier vs LTV |
| **Conversion** | Full funnel from install to 5th renewal, trial vs direct |
| **Retention** | Day 30, day 90, and 1-year retention by plan type |
| **Refunds** | Refund rates by plan type, region, and category |

Categories covered: Productivity, Utilities, Education, Health & Fitness, Photo & Video, Lifestyle, Graphics & Design, Entertainment.

Regions covered: North America, Europe, APAC, LATAM, MEA with country-level breakdowns.

## Source

All data is from the [Adapty State of In-App Subscriptions 2026](https://adapty.io/state-of-in-app-subscriptions-report/) report, covering 2025 transaction data.

## License

MIT
