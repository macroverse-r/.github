## Purpose

Briefly describe what this PR does and why.

## Related issues

Link related issues. Use `Closes #123` to auto-close on merge, `Fixes #123` for bugs, or `Related to #123` for loose connections.

## Type of change

- [ ] Bug fix
- [ ] Refactoring (no behavior change)
- [ ] New feature
- [ ] Documentation only

### Does this introduce a breaking change? (affects users of exported APIs)

- [ ] Yes -- describe the migration in the Purpose section
- [ ] No

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
