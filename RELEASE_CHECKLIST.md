# Release checklist — v7.4

## Frozen manuscript

- [x] Theorem/proof audit complete.
- [x] Prior-art boundary tightened for Schröder/Richardson/Romberg.
- [x] Lacunary-series context added (Zygmund, Kahane, Katznelson).
- [x] Nowhere-real-analytic theorem proved internally.
- [x] Numerical flat-gap table labelled illustrative only.
- [x] LaTeX build clean: no warnings, overfull boxes, or undefined references.
- [x] PDF render visually checked.

## GitHub preparation

- [ ] Choose repository name.
- [ ] Create repository as **private** initially if public timing is undecided.
- [ ] Upload the exact files in this release package.
- [ ] Verify GitHub renders `README.md` and `CITATION.cff` correctly.
- [ ] Decide whether to add a license. Do not infer one by default.
- [ ] Optionally create a signed/tagged release after public timing is chosen.

## Formal publication preparation

- [ ] Choose public-release date.
- [ ] Decide arXiv category/submission timing.
- [ ] Decide Zenodo timing and metadata.
- [ ] Add DOI to `CITATION.cff` and README only after one is assigned.
- [ ] Cross-link GitHub, Zenodo, ORCID, and the framework manuscript after publication.

## Final public-release checks

- [ ] Recompute SHA-256 hashes if any release file changes.
- [ ] Confirm PDF title, author, version, and date.
- [ ] Confirm bibliography and DOI strings.
- [ ] Confirm repository visibility before announcing the work.