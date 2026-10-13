# Mail-Driven Design

Start with the outcome, align on it with the user, then build the smallest useful thing that delivers it.

This repository packages one portable [Agent Skill](https://agentskills.io/) and a Claude Code plugin marketplace entry. The skill guides an agent to coauthor a short celebration email that makes the intended achievement and reader benefit concrete, get the user's alignment before implementation, and then implement and verify that promise. It contains no project-specific email or recipient information.

## Install

### GitHub Copilot and other Agent Skill hosts

Preview the skill, then install it with GitHub CLI 2.90.0 or later:

```sh
gh skill preview OmerMicro/mail-driven-design mail-driven-design
gh skill install OmerMicro/mail-driven-design mail-driven-design
```

`gh skill` is in public preview and requires GitHub CLI 2.90.0 or later. The skill follows the open Agent Skills format; hosts that support that format may use it, but availability and behavior depend on each host. See the [GitHub skill installation guide](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills).

### Claude Code

Add the marketplace, then install the plugin:

```sh
claude plugin marketplace add OmerMicro/mail-driven-design
claude plugin install mail-driven-design@mail-driven-design
```

The plugin includes the same skill. Review the plugin contents before installing it. See [Claude Code's marketplace guide](https://code.claude.com/docs/en/plugin-marketplaces).

## What it does

1. Coauthor an email that states the intended result, who benefits, and why it matters.
2. Get user alignment on that promise before implementation.
3. Turn the promise into a focused scope and verifiable acceptance criteria.
4. Implement the smallest useful solution, validate it, and report actual results for the user's final review.

The agent chooses a genuinely editable coauthoring surface available in its environment. If none is available, it uses a plain-text or Markdown draft in the user's editor; it does not require a particular app or canvas.

The skill does not send email, publish, merge, or perform other external actions without the user's explicit approval for the exact action and content. It distinguishes planned outcomes from verified results.

**Illustrative draft only — not a claim about completed work**

> **Subject:** One clear view of the next steps
>
> We're bringing next steps and owners into one shared view so teammates can see what's moving and where help is needed. The result we want is less time chasing updates and more time finishing work together.

## Repository layout

- `skills/mail-driven-design/SKILL.md` — portable Agent Skill
- `.claude-plugin/plugin.json` — Claude Code plugin manifest
- `.claude-plugin/marketplace.json` — marketplace catalog

## License

MIT. See [LICENSE](LICENSE).
