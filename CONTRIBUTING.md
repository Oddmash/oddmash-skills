# Install and maintain

Clone this repository into a stable local path. From the checkout, use Python 3.9 or later to run `python3 scripts/install.py` and link all shared skills into `~/.agents/skills`. Use `--target ~/.codex/skills` for an existing installation in that directory. Run the command with `--check` to check the destination without writing. [Codex local skill discovery](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)

For a product without a local copy, install the product playbook into its project skill directory, for example:

```sh
python3 scripts/install.py --product kowrap --target /path/to/kowrap/.agents/skills
```

The installer refuses collisions, including broken links. Back up an existing skill directory outside all discovery roots before converting it to a link. Start a new Codex session after installation. Updates to already linked skills are immediately visible through the links. After adding new shared skills, rerun the installer to create their links. Review updates before pulling them. The links depend on this clone's location.

Oddmash UI and Vertactics already ship their own project skills. Their central versions are available for review here while the original project paths remain active. Use one active copy of each skill. To adopt a revised central playbook in a product repository, review its differences in that repository and update its local copy in a product PR. Product-specific setup and approval requirements stay in that repository.

## Checks

```sh
python3 -m unittest discover -s tests
python3 scripts/install.py --validate
```

The validator checks the repository's manifest conventions, names, and relative skill links. Use the Codex skill creator's validator and review realistic activation scenarios when adding or materially changing skills.

## Initial source inventory

Shared skills began as the five locally installed Oddmash Codex skills. The product playbooks were reviewed against [Oddmash UI](https://github.com/Oddmash/oddmash-ui/tree/edcc43b0bab3e33662eb32c916a93fc2cc2780c9) and [Vertactics](https://github.com/Oddmash/Vertactics/tree/c011a0fba3b91ebbf9394771a547afbac7cd0bef). The [Kowrap playbook](products/kowrap/kowrap-landing/SKILL.md) captures typography and viewport checks exercised in the [landing renewal](https://github.com/Oddmash/kowrap/pull/7).
