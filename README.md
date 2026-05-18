# amlmarketplaces/zoom

Claude Code marketplace federating all `@amlplugins/zoom-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-zoom": {
      "source": { "source": "github", "repo": "amlmarketplaces/zoom" }
    }
  },
  "enabledPlugins": {
      "zoom-video-sdk@aml-zoom": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/zoom`, cached under `~/.claude/plugins/cache/aml-zoom/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (1 total)

- `zoom-video-sdk` — [@amlplugins/zoom-video-sdk](https://github.com/amlplugins/zoom-video-sdk)

## Related

- npm packages: `@amlplugins/zoom-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
