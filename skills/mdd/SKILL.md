---
name: mdd
description: Mail-Driven Design (MDD). Coauthor an outcome-focused celebration email, align with the user before implementation, then build and verify the promised result. Use for /mdd, mail-driven-design, or starting a project, feature, or substantial change where the intended outcome should be clear before work begins.
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

Keep one user-editable canonical draft in the best native editor or genuinely editable surface available. Do not require a particular app, Word document, or canvas. Fall back to a plain-text or Markdown file in the user's editor. Use approval questions for decisions, never as the container for a full draft.

Reread the canonical draft before each revision or requested synchronization. Preserve the user's exact wording and untouched sections, including bullets, line breaks, emojis, and code blocks. Apply only the requested changes; do not offer an unsolicited full rewrite. If mailbox and canonical edits conflict, reconcile them with the user rather than overwriting either. When the user requests a public repository example, synchronize it from the latest reviewed draft, excluding private recipients and context; do not maintain a divergent marketing rewrite.

Get explicit alignment on the email's promise before implementation. Track draft approval, implementation approval, and send approval separately; none implies the others. Sending always requires separate approval of the exact final content and the send action.

### Only when mailbox synchronization is requested

Use supported native mail tools and the user's authorized scope. Read the existing mailbox draft first and preserve its edits and recipients. Resolve requested recipients, especially distribution lists, to exact addresses through an authoritative directory or existing message metadata. Never silently drop unresolved recipients or substitute individuals for a requested list; surface unresolved names and do not call the draft ready to send.

Convert the canonical draft to the mailbox's supported format faithfully. For Markdown-to-HTML conversion, preserve wording and formatting, including lists, line breaks, emojis, and code blocks. After saving, reread the persisted body and recipients to verify the intended result. If verification is unavailable or fails, report that gap instead of claiming synchronization succeeded. Saving a draft does not authorize sending it.

## 3. Turn the promise into a small plan

After the user aligns on the email, extract:

- The outcome and intended beneficiary.
- Observable acceptance criteria that show whether the outcome was delivered.
- The smallest scope that can deliver the promise.
- Explicit non-goals, assumptions, and dependencies that matter.

Use repository and project context to check feasibility and identify relevant existing patterns. Keep the work focused; do not add infrastructure, workflows, or abstractions without a concrete need. If a material ambiguity remains, resolve it before making a consequential design choice.

## 4. Implement toward the agreed outcome

Make small, cumulative changes that directly serve the aligned promise. Reuse existing capabilities and conventions. Keep the user informed when evidence changes the plan or reveals a meaningful tradeoff; incorporate feedback without overwriting unrelated user work.

Delegate only when expertise, parallelism, or a separate context materially helps. Give any delegated agent the aligned promise, scope, constraints, and evidence required for completion. Otherwise do the work directly; do not add orchestration just to follow this workflow.

Respect the user's authority. Do not send messages, publish, merge, spend money, change access, or perform other consequential external actions unless the user explicitly approves the exact action and its scope. Preparing a draft or implementation does not authorize that action.

## 5. Verify and bring back the result

Run the smallest relevant checks that demonstrate the acceptance criteria. Inspect the resulting behavior or artifact where practical. Report:

- What is actually implemented.
- What evidence verifies it.
- What remains incomplete, uncertain, or dependent on external input.

Keep intended outcomes, implementation status, and verified results distinct. Do not claim the email's promise was fulfilled until the evidence supports that conclusion. Return the actual result for the user's final review.

When installation or distribution is part of the promise, provide real commands and precise host support. Distinguish documented syntax from an installation actually verified. Do not leave placeholders in a ready-to-send draft; disclose unresolved installation details.
