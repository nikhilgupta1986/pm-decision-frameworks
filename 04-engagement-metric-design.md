# Designing & Measuring Engagement Features

## The situation this solves

You're building something meant to change user behavior, a gamification layer, a nudge system, an insights feed, and you need to define success before you ship, not after. "Engagement went up" isn't a metric, it's a vibe. Points collected isn't a metric either, it's a vanity number that can go up while the actual behavior you care about goes nowhere.

## The framework

Define layers of metrics, from the outcome you actually care about down to the diagnostics that explain it:

1. **The core outcome metric: meaningful engagement rate.** `Users completing a meaningful action / eligible monthly active users x 100`. A "meaningful action" has to be defined upfront and tied to real value, not just any click. Examples: creating or updating a budget, acting on a nudge, completing a financial-literacy chapter.
2. **Uplift, measured properly.** Before/after: `(post-launch rate - pre-launch rate) / pre-launch rate x 100`. Or, better, with an experiment: `(treatment rate - control rate) / control rate x 100`. Report relative uplift alongside absolute percentage-point change, they tell different stories and both matter.
3. **Supporting metrics that explain the outcome, not replace it:** activation rate (users taking the first meaningful step / eligible users), review/repeat rate (are people coming back, or was this a one-time action?), nudge action rate (users acting on a specific prompt / users who received it, within a defined time window), and completion vs. adherence (finishing a flow is feature engagement; staying within budget is a real customer outcome, these are different things).
4. **Treat surface-level metrics (points, streaks, badges) as diagnostic only, never as the headline result.** Users can rack up points without the underlying behavior actually improving. If points are the only number you report, you likely haven't measured what you think you've measured.

## How I've used it

At Sopra, I personally designed a gamification layer for a personal finance product, interactive challenges, rewards, and financial-literacy content, aimed at improving real financial behavior, not just clicks. I built this metric structure to define what success would actually mean before launch.

Being direct about a limitation here: I don't have a real, remembered engagement-lift number from this specific feature to report. What I have is the framework itself, which is the reusable part. A separate feature I shipped in the same role, an AI-powered personalized financial newsfeed, did have a measured outcome: per client feedback, the bank reported cross-sell and up-sell conversions doubled within 6 months. I'm keeping these two examples separate rather than blending them, since attaching one feature's real result to a different feature's description would misrepresent what was actually measured.

## When this framework breaks down

If you don't have a clean way to define "eligible users" or can't run a proper before/after or control comparison (small sample size, no experimentation infrastructure), the uplift numbers this framework produces will be noisy or misleading. In that case, report the framework's structure honestly and flag that the sample or method limits confidence in the specific number, rather than presenting a shaky calculation as a clean result.
