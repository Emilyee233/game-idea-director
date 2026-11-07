# Release Checklist

## Structure
- [ ] Canonical folder is `game-idea-director/`.
- [ ] Frontmatter `name` matches folder.
- [ ] Every path in `reference-index.md` exists.
- [ ] No planned file is presented as available.
- [ ] No duplicate `SKILL.md`.

## Behavior
- [ ] Should-trigger routing cases pass.
- [ ] Should-not-trigger cases pass.
- [ ] Missing expertise is disclosed.
- [ ] Proposals are not silently promoted to confirmed decisions.
- [ ] Exact numerical claims have adequate basis.
- [ ] Test/research/action claims require evidence.

## Privacy
- [ ] No private project names/content in public files.
- [ ] No local absolute paths.
- [ ] No credentials/secrets/private URLs.
- [ ] Examples are independently fictional.
- [ ] Git history reviewed before public release. For a brand-new repository, verify the staged first commit contains only the audited V1.0 snapshot.

## Packaging
- [ ] README explains scope and limits.
- [ ] INSTALL is current.
- [ ] CHANGELOG updated.
- [x] MIT LICENSE included.
- [ ] Release archive installs using the inner canonical folder.
