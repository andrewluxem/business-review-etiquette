# business-review-etiquette

Turns supplied review material into an evidence-bound participation brief and etiquette audit.

It produces:

- **Business Review Participation Brief or Business Review Etiquette Audit:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Business Review Etiquette playbook](https://www.andrewluxem.com/playbooks/business-review-etiquette). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/business-review-etiquette.git
cp -r business-review-etiquette/skills/business-review-etiquette ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r business-review-etiquette/skills/business-review-etiquette ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/business-review-etiquette
/plugin install business-review-etiquette@business-review-etiquette
```

For clients that install from an archive, use the versioned [business-review-etiquette v1.0.0 ZIP](https://www.andrewluxem.com/downloads/business-review-etiquette-v1.0.0.zip).

## Invoke it

```text
Audit this business review for participation discipline
Use the business-review-etiquette skill.
```

Naming the skill is always valid: `use the business-review-etiquette skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/business-review-etiquette/
  assets/business-review-participation-brief-template.md
  LICENSE.md
  meta.yaml
  references/participation-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/business-review-etiquette/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/business-review-etiquette/LICENSE.md](skills/business-review-etiquette/LICENSE.md).
