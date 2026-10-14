# Tools

- `build_map.py` checks the entries against the schema and writes `MAP.md`.
- `build_bundle.py` writes `map-bundle.md`.
- `count_sources.py [FOLDER]` prints the counts of sources quoted on the site and in the README (source references, distinct URLs, primary and third-party-only URLs, distinct URLs in the bundle) and a `[SCOPE]` line saying what it does not count.
- `build_site.py` writes the static site (one page per entry, notes, graph, `map.json`, `calendar.ics`).

## Publishing the site

The footer and the "verified" stamp link to a commit only if that commit exists in this repository. Build the site from this repository itself, after the data are committed:

1. Commit the data (entries, notes, README, bundle) on `main`.
2. Build the site from the folder of this repository, so that the commit shown is the commit of the data:
   `python tools/build_site.py --source . --out docs --base-url https://frmoretto.github.io/agentic-standards-map/`
   Add `--doi <DOI>` (and, if wanted, `--cite-version <version>`) once the dataset has a DOI: the author block then carries a "How to cite" section. Without `--doi` nothing about citation is shown.
3. Restore `docs/.nojekyll` (the build clears the output folder) and commit `docs/` in a separate commit.

Without `--source` the script exports the data from a commit of the working repository and shows no commit link, only a link to the repository, because a commit of the working repository does not exist here.

The author block of the site is generated from the constants at the top of `build_site.py` (`AUTHOR`, `ORCID`, `GITHUB`, `LINKEDIN`, `ISSUES_URL`); `README.md` carries the same text and the build stops if the README lacks one of the constants. After a DOI is issued, add the "How to cite" section to the README by hand with the same wording.
