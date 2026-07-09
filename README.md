# reUrgency Marketplace

One storefront for **reUrgency**'s tools — built to make AI-assisted engineering faster and
more reliable across **Claude Code, Codex, Cursor, and GitHub Copilot**.

Add the marketplace once, then install any product from it.

```bash
/plugin marketplace add reurgency/marketplace
/plugin install <plugin>@reurgency
```

Update everything later with `/plugin marketplace update reurgency`.

## Products

| Plugin | What it does | Install |
|---|---|---|
| **[deep-skills](https://github.com/reurgency/Deep-Skills)** | The Deep-* series — planning → review → implementation → code-review → bug-fix → docs as one coherent, fresh-agent-resumable workflow, with a self-improving directive loop. | `/plugin install deep-skills@reurgency` |
| **[overton-snapshot](https://github.com/reurgency/Overton-Snapshot)** | Scenario-aware context snapshots for zero-context agent handoffs, plus a context-usage statusline and an over-threshold nudge. | `/plugin install overton-snapshot@reurgency` |
| **[sym-visualizer](https://github.com/reurgency/Sym-Visualizer)** | Find every symlink under a folder and turn it into a Markdown report, a CSV table, and a self-contained interactive graph. | `/plugin install sym-visualizer@reurgency` |

Each product's code lives in its own repo; this repo is just the catalog that points at them.
Full per-host install commands and capability matrices live in each product's README.

## Migrating from an older install

Earlier releases were published under per-product marketplace names (`deep-skills-by-reu`,
`cc-plugins-by-reurgency`, `reurgency-plugins`). Those are retired in favor of this single
storefront. To switch:

```bash
# remove the old marketplace (use whichever you had)
/plugin marketplace remove deep-skills-by-reu
/plugin marketplace remove cc-plugins-by-reurgency
/plugin marketplace remove reurgency-plugins

# add the new one and reinstall
/plugin marketplace add reurgency/marketplace
/plugin install <plugin>@reurgency
```

Your existing install keeps working until you switch — migrate whenever it's convenient.

## License

MIT © reUrgency
