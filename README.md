# iOS Monetization Expert — Claude Code Skill

A Claude Code skill that turns Claude into an expert iOS subscription monetization advisor. It gives direct, benchmarked advice grounded in real data from Adapty's State of In-App Subscriptions 2026 report ($3B revenue, 16,000+ apps).

## What It Does

When you ask monetization questions in Claude Code, this skill automatically activates and provides:

- **Instant benchmarking** — Compare your metrics (LTV, conversion, retention, churn) against industry data
- **Pricing guidance** — Region-specific pricing benchmarks across weekly, monthly, and annual plans
- **Trial strategy** — Whether to use free trials based on your category and plan type
- **Growth advice** — Which markets to target, when to raise prices, how to reduce churn
- **Direct answers** — No fluff, just what the data says and what you should do next
- **LTV Prediction Calculator** — Interactive calculator that projects your LTV, revenue, and breakeven timeline based on your subscription plans, pricing, and conversion data

## LTV Prediction Calculator

Tell Claude your subscription plans, pricing, and metrics — it runs the full LTV model and tells you whether your app will be profitable.

**What you provide:**
- Subscription plans (type, price, distribution %)
- Monthly installs, CR to purchase, CPI
- Trial funnel data (trial start rate, trial-to-paid rate) if you use free trials
- Retention data (optional — defaults to industry benchmarks)

**What you get:**
- LTV, ARPU, and revenue projections across 8 time horizons (7d → 4yr)
- ROAS and breakeven timeline
- LTV:CAC ratio and unit economics assessment
- Performance grades vs industry benchmarks
- Specific advice on pricing, plan mix, trial optimization, and retention
- "What-if" scenario modeling (e.g., "what if I raise prices 30%?")

**Example prompt:**
> "I have an app with annual ($89.99, 25%), quarterly ($39.99, 35%), monthly ($19.99, 35%), lifetime ($99, 5%). My CR is 6%, CPI is $3, 40k installs."

## Example Questions

- "How should I price my Health & Fitness app?"
- "How many free trial days should I offer?"
- "Should I add a weekly plan?"
- "Should I use a free trial or a direct paywall?"
- "Which countries should I target for the best LTV?"
- "What's a good install-to-paid conversion rate?"
- "How do I reduce churn on my annual plan?"
- "Will my app be profitable?"
- "What if I improve my trial-to-paid conversion from 20% to 30%?"

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
| **LTV Prediction** | Revenue projections, ROAS, breakeven, LTV:CAC, scenario modeling |
| **Trial Funnel** | Trial start rate and trial-to-paid benchmarks with assessment thresholds |

Categories covered: Productivity, Utilities, Education, Health & Fitness, Photo & Video, Lifestyle, Graphics & Design, Entertainment.

Regions covered: North America, Europe, APAC, LATAM, MEA with country-level breakdowns.

## Source

All data is from the [Adapty State of In-App Subscriptions 2026](https://adapty.io/state-of-in-app-subscriptions-report/) report, covering 2025 transaction data.

## License

MIT
