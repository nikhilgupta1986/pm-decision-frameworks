# Diagnosing Low Adoption

## The situation this solves

You shipped something you believed in, and people aren't using it. The instinct is to treat this as one problem, usually "the tool isn't good enough yet", and iterate on the product. That instinct is often wrong, or at least incomplete.

## The framework

1. **Don't assume a single cause. Talk to the actual non-adopters, one on one.** Not a survey, a real conversation. Aggregate feedback ("people say it's not accurate enough") often hides two or more distinct problems being reported as one.
2. **Separate technical trust problems from human/organizational ones.** A tool can be distrusted because it's been wrong before (a technical, fixable problem: add traceability, improve accuracy). It can also be resisted because people fear what it means for their role (a human problem that no amount of accuracy improvement fixes on its own).
3. **Fix each cause with the tool that actually matches it.** Traceability and explainability address trust in the output. Explicit reassurance, changed process design (e.g., stricter human-approval gates), and direct conversation address fear of displacement. Using only one kind of fix when both problems exist means half the resistance never goes away.
4. **Reframe the tool's purpose explicitly, don't assume the reframe is obvious.** If the tool is meant to make people faster at their own job, not replace their judgment, say that directly and build the workflow to prove it (e.g., "nothing proceeds without your approval").

## How I've used it

When we launched a GenAI Underwriting Co-Pilot at Perfios, adoption was low, underwriters kept doing everything manually. I found two separate causes, not one: some early recommendations had been wrong and eroded trust, and separately, underwriters worried the tool was designed to make their role redundant. I talked to them directly rather than assuming it was purely an accuracy problem.

From that, two different fixes: I added output traceability so underwriters could see why a recommendation was generated, and I made the human-in-the-loop review step explicitly stricter, "nothing proceeds without your approval", while also making the case directly that the tool's purpose was to make them faster at their own judgment, not to replace it.

Result: adoption increased, and the co-pilot became part of underwriters' standard operating procedure.

## When this framework breaks down

If you can't get honest access to the non-adopters (they've disengaged, or there's a power dynamic that keeps them from telling you the real reason), this framework requires information you might not be able to get directly. In that case, look for proxy signals, usage patterns, exit points in the workflow, indirect feedback through their manager, rather than assuming silence means "it's an accuracy problem" by default.
