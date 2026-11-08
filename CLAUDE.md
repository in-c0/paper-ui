# paper-ui

Rules live in one place: [in-c0/Project-harness](https://github.com/in-c0/Project-harness) —
`POLICY.md` (what a session may do), `INFRA.md` (what is already provisioned), `NEEDS_JI.md`
(the only hand-back queue). Read `POLICY.md` before acting. This file carries no policy of its
own; only the facts below.

## This repo
- Independent React component library (not a Tegaki fork; never vendor Tegaki or Paper Shaders code). Semantic DOM + one optional shader layer with CSS fallback; never one WebGL canvas per list item.
- Preserve the six owner-approved shader presets exactly (alpha hex values, numeric zeros, seed 893). Accessible, keyboard-usable, reduced-motion aware.
- Release gate (product rule): "production-ready" and an npm publish need tests for mobile layout, WebGL compat, keyboard, screen readers, visual regression, low-power devices; new deps need a license/maintenance note. `npm-alpha-stage.yml` is the alpha channel.

Earlier rule files for this repo are archived under `docs/archive/rules/2026-11-08/` and expire
on 2027-02-06 (POLICY.md §8). Open one only if something in this repo stops making sense
without it, and if you did, say which file in your PR description in one line.

Reply to the owner in Korean. Code, commit messages and PR text stay in English.
