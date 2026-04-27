## Purpose

Briefly describe what this PR does and why.

## Related issues

Link related issues. Use `Closes #123` to auto-close on merge, `Fixes #123` for bugs, or `Related to #123` for loose connections.

## Type of change (pick one primary)

- [ ] Bug fix -- restores documented behavior; no API change
- [ ] Feature -- new user-facing capability (new function, argument, behavior)
- [ ] Refactor / internal -- reorganization, performance, internal helpers; no API change
- [ ] Documentation -- roxygen, vignettes, README, NEWS only
- [ ] Infrastructure -- `.github/`, `.claude_macroverse/`, CI, build, repo tooling

## Flags (tick all that apply)

- [ ] API change -- adds, renames, removes, or alters signature of any exported function
- [ ] Breaking change -- downstream packages need code changes
- [ ] Cross-package coordination -- touches a shared workspace or needs coordinated release

## Checklist

- [ ] PR is focused on one theme (no unrelated changes bundled in)
- [ ] Tests added or updated in `tests/testthat/` for the behavior I changed
- [ ] `devtools::check()` is clean (0 errors, 0 warnings)
- [ ] `NEWS.md` bullet added for user-facing changes, format: `* Description. (@username, #PR)`
- [ ] roxygen2 docs and `man/` regenerated if exported signatures changed
- [ ] Follows DRY and simplicity: no duplication with existing macroverse functions, no re-implementation of logic already available (verified via `rfunsig`, `.funnet()`, `.pkgnet()`, or similar)
- [ ] Cross-package effects checked (if changing an `mv_*`, `im_*`, `md_*`, etc. consumed by siblings)

## Follow-up work needed

Link issues for work that is out of scope for this PR -- either newly opened for the purpose, or pre-existing issues that remain open after merge.
