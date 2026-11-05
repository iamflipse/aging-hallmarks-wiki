# Hallmarks of Aging — Wiki

A curated wiki distilling the 2026 *International Journal of Molecular Sciences* review:
**The Hallmarks of Aging: From Molecular Mechanisms to Clinical Translation**
(Chmielewski & Strzelec, IJMS 2026;27(18):8080, open access CC-BY, DOI 10.3390/ijms27188080).

**Public copy:** https://iamflipse.github.io/aging-hallmarks-wiki/ (read-only; static build served from the `gh-pages` branch)

## Contents

- **12 hallmark pages** (genomic instability → dysbiosis & barrier dysfunction), each traced to the paper's sections §2–13
- [Candidate processes (RNA, ECM)](src/concepts/candidate-processes.md) — §14
- [Causal-module framework](src/concepts/causal-modules.md) — §15 (four-question appraisal, network feedback)
- [Clinical translation program](src/concepts/clinical-translation.md) — §16
- **Full text** at `src/sources/ijms-27-18-8080-fulltext.md` (195 KB, 161 references)

## Layout

- `src/` — markdown source pages
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish: recreate orphan gh-pages branch with book files at root, force push
```
