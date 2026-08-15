## What changed

<!-- One or two sentences. If this fixes drift, name the command or concept. -->

## Verified against

- `bd version`:
- How verified (commands run, or "docs only"):

<!--
Anything about CLI behavior should be checked against a real binary in a temp
workspace, not inferred from docs:

  d=$(mktemp -d); ( cd "$d" && git init -q && bd init --quiet --prefix test ); rm -rf -- "$d"

Reminder: `bd help <unknown>` exits 0. Test existence with
`bd foo --help 2>&1 | head -1`.
-->

## Checklist

- [ ] `./scripts/validate.sh` passes
- [ ] `SKILL.md` only changed if agent *behavior* should change
- [ ] Anything absent from the pinned `bd` version is marked, not omitted
- [ ] Nothing from `beads/` is committed (submodule pointer only)
- [ ] `BEADS_VERSION.md` updated if the pin or known drift changed
- [ ] `CHANGELOG.md` updated under Unreleased
