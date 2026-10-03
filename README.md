# cli-release-versioning

Releasing by hand is where version numbers go wrong — a forgotten `VERSION` file, a changelog nobody wrote,
a release branch cut from the wrong commit. This is the command line tool that does the whole sequence in one
step, the same way every time.

## What it is for

One command that:

- creates the release branch for the kind of release you are cutting — **patch**, **minor** or **major**;
- updates the `VERSION` file to match;
- commits and pushes to git;
- prepares `CHANGELOG.md` for the entries that belong to that release.

## Status

**The package manifest is in place; the command itself has not been published to this repository yet.**
`package.json` declares `main: index.js`, and that file is not here — the repository currently holds the
manifest and its ignore rules only. This README will be rewritten with real usage examples when the source
lands.

## Intended use

```bash
npx @nodejavascript/cli-release-versioning patch
npx @nodejavascript/cli-release-versioning minor
npx @nodejavascript/cli-release-versioning major
```

## Licence

MIT.
