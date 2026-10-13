# Mail-Driven Design

**Write the celebration email first. Align on it. Build to that promise.**

📧 **Coauthor** → 🤝 **Align** → 🛠️ **Build** → 👀 **Your final review**

[Install](#install) · [Try it](#try-it) · [Read the skill](skills/mdd/SKILL.md) · [Contribute](#contribute)

## The email that started this repo

This repository was built using MDD: we coauthored the launch email, aligned on the promise, then delegated implementation. Here is the public-safe core of that email, not a claim that the launch or final review is complete:

> **Subject: MDD: Mail-Driven Design**
>
> Hi!
>
> I’m writing the “we shipped it” email before writing the code. Slightly backwards, but hopefully less backwards than shipping something nobody asked for.
>
> **MDD - Mail Driven Design**
>
> First, write the celebration email: what you achieved, how it helps the reader, and how it makes things better for humankind 🧑‍🚀.
> Then delegate the work and build to that promise 👨‍💻.
> The agent brings the result back to you for your final review 🎉.
>
> 📧 Write the celebration email → 🛠️ Delegate and build → 👀 Your final review → 🏆 Milestone achieved, impact visible, Hall of Fame seat reserved
>
> **Install in a click of a prompt** 😉
>
> Try it out!
> Contributions are more than welcome!
>
> Like and subscribe. 👍

The email defines the intended win. User alignment comes **before implementation**; evidence comes **before claiming success**. Delegation is optional when one agent can do the work.

## Install

One [Agent Skill](https://agentskills.io/specification), packaged for plugin marketplaces. **No runtime, dependencies, hooks, or servers.** Choose one route; you do not need both a plugin and a standalone skill.

<details open>
<summary><strong>GitHub Copilot CLI: marketplace → plugin</strong></summary>

```sh
copilot plugin marketplace add OmerMicro/mail-driven-design
copilot plugin install mail-driven-design@mail-driven-design
```

</details>

<details>
<summary><strong>Claude Code: marketplace → plugin</strong></summary>

```sh
claude plugin marketplace add OmerMicro/mail-driven-design
claude plugin install mail-driven-design@mail-driven-design
```

</details>

<details>
<summary><strong>Standalone skill: Copilot or another Agent Skill host</strong></summary>

With GitHub CLI 2.90.0 or later (`gh skill` is in public preview):

```sh
gh skill preview OmerMicro/mail-driven-design mdd
gh skill install OmerMicro/mail-driven-design mdd
```

The default is a project-scoped Copilot skill. Use `gh skill install --help` to choose another host or scope. Without GitHub CLI, copy the `skills/mdd` directory into your host's documented skills directory.

</details>

Review [the skill](skills/mdd/SKILL.md) before installing. Commands follow the [Copilot](https://docs.github.com/en/copilot/how-tos/copilot-cli/customize-copilot/plugins-marketplace), [Claude Code](https://code.claude.com/docs/en/plugin-marketplaces), and [GitHub CLI](https://cli.github.com/manual/gh_skill_install) documentation.

## Try it

Ask your agent:

```text
/mdd Let's coauthor the celebration email for this project and align
on the outcome before you implement anything.
```

**Copyable installation prompt** (for an agent with plugin support):

```text
Review https://github.com/OmerMicro/mail-driven-design. Using this host's
documented plugin commands, add its marketplace and install the
mail-driven-design plugin. Marketplace name: mail-driven-design.
If plugins aren't supported, explain the standalone skill option first.
```

The skill is named **`mdd`** so Copilot can find it when you type `/mdd`. In Claude Code, use `/mail-driven-design:mdd` for the plugin or `/mdd` for a standalone skill. Other hosts may use different invocation or suggestion rules.

The agent chooses an editable coauthoring surface available to it, with a plain-text or Markdown file in your editor as the fallback. No special app or canvas required. It preserves your edits and returns the actual result for your final review.

**Drafting is not sending.** Sending an email always needs separate approval of the final content and the send action. A success promise is not evidence that it happened.

## Compatibility

| Surface | Verified | Not yet verified |
| --- | --- | --- |
| Agent Skill / GitHub CLI | Skill validation and remote preview | Full workflow in each host |
| GitHub Copilot CLI | Local plugin discovery without installing | Marketplace installation and full workflow |
| Claude Code | Strict plugin and marketplace validation | Installation and full workflow |

Portable instructions do not guarantee identical behavior across hosts. These are packaging checks, not proof of downstream impact. Final review is still pending.

## Contribute

[Open an issue](https://github.com/OmerMicro/mail-driven-design/issues) for a concrete improvement or compatibility problem. Small, focused pull requests are welcome; include the host and version, what you tried, and what you observed. Keep the workflow portable and dependency-free.

MIT licensed. See [LICENSE](LICENSE).
