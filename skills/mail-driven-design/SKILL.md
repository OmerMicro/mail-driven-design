---
name: mail-driven-design
description: Coauthor an outcome-focused celebration email, align with the user before implementation, then build and verify the promised result. Use when starting a project, feature, or substantial change where the user wants the intended outcome made clear before work begins.
license: MIT
---

# Mail-Driven Design

Use the email as a compact agreement about the outcome—not as a substitute for planning, implementation, or evidence. The email is the first deliverable; the implemented result is the main one.

## 1. Understand the intended win

Start by understanding why the work matters:

- What should be different when the work is done?
- Who benefits, and what becomes easier or better for them?
- What would make the user say the effort was worthwhile?

Use what the user has already said. Ask only for missing information that would materially change the outcome, scope, authority, or feasibility. Do not make the user repeat known context or complete a long questionnaire.

## 2. Coauthor the email first

Draft a concise, forward-looking email that makes the intended achievement, reader benefit, and outcome concrete. Keep future promises clearly aspirational; never describe planned work as already achieved.

Use the best genuinely editable coauthoring surface available in the current environment. Do not assume a particular app, canvas, or integration. If no suitable surface exists, provide a plain-text or Markdown draft the user can edit in their own editor. Do not put a full draft into a question or approval prompt when a better editing surface is available.

Invite the user to review and revise the draft. Apply their feedback surgically: preserve edits and sections they did not ask to change. Get explicit alignment on the email's promise before starting implementation. Do not send the email; sending requires separate approval of both the exact final content and the send action.

## 3. Turn the promise into a small plan

After the user aligns on the email, extract:

- The outcome and intended beneficiary.
- Observable acceptance criteria that show whether the outcome was delivered.
- The smallest scope that can deliver the promise.
- Explicit non-goals, assumptions, and dependencies that matter.

Use repository and project context to check feasibility and identify relevant existing patterns. Keep the work focused; do not add infrastructure, workflows, or abstractions without a concrete need. If a material ambiguity remains, resolve it before making a consequential design choice.

## 4. Implement toward the agreed outcome

Make small, cumulative changes that directly serve the aligned promise. Reuse existing capabilities and conventions. Keep the user informed when evidence changes the plan or reveals a meaningful tradeoff; incorporate feedback without overwriting unrelated user work.

Respect the user's authority. Do not send messages, publish, merge, spend money, change access, or perform other consequential external actions unless the user explicitly approves the exact action and its scope. Preparing a draft or implementation does not authorize that action.

## 5. Verify and bring back the result

Run the smallest relevant checks that demonstrate the acceptance criteria. Inspect the resulting behavior or artifact where practical. Report:

- What is actually implemented.
- What evidence verifies it.
- What remains incomplete, uncertain, or dependent on external input.

Keep intended outcomes, implementation status, and verified results distinct. Do not claim the email's promise was fulfilled until the evidence supports that conclusion. Return the actual result for the user's final review.
