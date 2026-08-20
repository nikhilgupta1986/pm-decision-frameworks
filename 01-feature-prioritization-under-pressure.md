# Feature Prioritization Under Pressure

## The situation this solves

Someone with real influence, a Head of Sales, an exec, a big customer, asks you to add a feature into a release that's already committed and on track. Saying yes without a framework is how scope creep happens. Saying no on instinct risks a bad call and a damaged relationship. Neither "just do what leadership wants" nor "protect the roadmap at all costs" is actually a decision, they're defaults.

## The framework

Before answering, get real answers to four questions:

1. **What problem does this actually solve, and for whom?** A vague "customers want this" isn't an answer. Get specific: which customer, what pain, how painful.
2. **Is the demand validated or assumed?** Did a customer explicitly ask for it, or did it surface in one internal conversation? These carry very different weight.
3. **Is it reusable across your base, or custom to one account?** This changes the ROI math significantly, a platform capability and a one-customer favor are not the same investment.
4. **What's the real cost of doing it now vs. later?** Not just the effort to build it, what does it displace? Every "yes" to something new is implicitly a "no" or "later" to something already committed.

## How I've used it

At Perfios, mid-way through a general release of our Loan Origination System, with the release on track, our Head of Sales asked me to add a new feature into the current release. I ran it through these four questions instead of deciding on gut feel. It turned out to be a one-customer custom request that had come up in a single sales meeting, not broad demand, and pulling it forward would have cost more (in delayed committed scope) than it was worth.

I presented the data, not my opinion, to the Head of Sales. He agreed. The release shipped on time. The request went into the backlog and was delivered in the next cycle, and the customer wasn't left hanging, since we told them upfront where it stood.

**Worth naming honestly:** saying no cost something. The relationship with that stakeholder was a little strained afterward. A good framework doesn't guarantee everyone leaves happy, it means the decision is defensible with data instead of authority, even when someone doesn't love the outcome.

## When this framework breaks down

It assumes you can actually get honest answers to all four questions quickly. If you can't get real customer-demand data (no CRM, no direct access to the requester's source), you're reasoning from incomplete information, and you should say so explicitly rather than pretend the framework gives you more certainty than it does.
