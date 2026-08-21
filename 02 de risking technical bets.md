# De-Risking a Technically Uncertain Bet

## The situation this solves

You have an idea that could be genuinely valuable, but you don't actually know if it's technically achievable. There's no internal precedent, no clear playbook. Committing the full roadmap to it is a bet, not a plan, but so is avoiding every uncertain idea until someone else proves it first.

## The framework

1. **Talk to the people who'd have to build it, before you commit anything.** Not for permission, for a rough, honest feasibility read. This is a cheap, fast way to convert vague uncertainty into a first real signal.
2. **Run the smallest possible proof of concept that would tell you if the core hypothesis holds.** Not a full build, the minimum thing that answers "is this fundamentally possible" before you answer "how good can we make it."
3. **Let the POC resolve the open technical questions you can't answer from a whiteboard.** Some things (which underlying approach to use, what the real failure modes are) only become clear once you've actually tried it.
4. **Decide what you're willing to accept if it doesn't work.** This is the step people skip. Know, going in, whether you have a fallback or whether you're accepting real risk with no safety net, and be honest with yourself and your stakeholders about which one it is.

## How I've used it

At Perfios, I pitched building an AI Workflow Builder, letting product and operations teams generate a working loan journey from a natural-language description instead of a multi-day engineering build. I genuinely didn't know if it was achievable. I talked to Engineering and Data Science first to gauge rough feasibility, then ran a small POC to test the actual open question: whether a general-purpose LLM or a domain-trained SLM would reliably produce correct backend rules. The POC is what resolved that, not the discussion beforehand.

I committed to the full build only after the POC validated the SLM approach. There was no fallback plan if it hadn't worked, that was a real risk I accepted knowingly, not one I quietly assumed away.

**Result:** custom loan-journey configuration and demo turnaround dropped from 7-9 days to 1-1.5 days.

## When this framework breaks down

If the POC is ambiguous, neither a clear yes nor a clear no, this framework doesn't tell you what to do next. That's a real gap: sometimes you have to make a second, smaller POC decision, or accept you're committing on weaker signal than you'd like. Don't let the structure make an ambiguous result feel more decisive than it is.
