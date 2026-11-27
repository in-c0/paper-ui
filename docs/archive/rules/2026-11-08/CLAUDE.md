# Paper UI contributor and coding-agent contract

- This is an independent React component library, not a Tegaki fork. Do not rename or claim ownership of Tegaki or Paper Shaders.
- Keep material rendering and controls separate: semantic DOM + one optional shader layer, with CSS fallback.
- Never render one WebGL canvas per list item.
- A gradient is not a physically accurate 3D lamp; handwriting stroke animation is not graphite physics.
- Preserve all six owner-approved shader presets, including alpha-bearing hex values, numeric zeros, and seed 893.
- Use original source files under packages/paper-ui; do not vendor or copy Tegaki or Paper Shaders code.
- Keep any UI component accessible, keyboard usable, and reduced-motion aware.
- Do not claim "production-ready" until tests cover mobile layout, WebGL compatibility, keyboard, screen readers, visual regressions, and low-powered devices.
- New dependencies need explicit maintenance/license audits.
- No registry, npm publishing, source release, or domain change without documented ownership and QA.
- Keep public README succinct, honest, and specific to Paper UI, not the original Tegaki repository.

## Merging pull requests

The repository owner (@in-c0) has pre-approved merges: when Claude opens a pull request in this repository, merge it as soon as its CI checks pass. Do not wait for a review and do not ask the owner for permission.

- Merge with `gh api -X PUT repos/in-c0/<repo>/pulls/<number>/merge -f merge_method=squash`. In cloud sessions `gh pr merge` fails because the GitHub proxy blocks GraphQL; locally `gh pr merge <number> --squash` also works. Both forms are allow-listed in `.claude/settings.json`.
- If the merge is still blocked (a permission check, branch protection or failing CI), tell the owner once, in one line, with the reason and the PR link. Do not repeat that message on later wake-ups.
- Reply to the owner in Korean. Code, commit messages and PR text can stay in English.
