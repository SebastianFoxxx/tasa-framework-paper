# TASA: A Tick-Based Affective State Architecture for Persistent, Inspectable Inner State – Framework, Learnability Conditions, Governance, and Evaluation

A specification-style framework paper for the TASA research programme.

## Status and identifiers

- Author: Sebastian Fuchs
- Affiliation: Institut für Informatik, Humboldt-Universität zu Berlin
- ORCID: [https://orcid.org/0009-0009-1237-4804](https://orcid.org/0009-0009-1237-4804)
- Contact: [sebastian.fuchs@hu-berlin.de](mailto:sebastian.fuchs@hu-berlin.de)
- Version: 1.0.0
- First publication: 2026-09-03
- Canonical archive: [https://doi.org/10.5281/zenodo.22283059](https://doi.org/10.5281/zenodo.22283059)
- arXiv: not announced

## Abstract

Standard language-model inference lacks cross-exchange internal organization. External memory can reconstruct continuity without persistent state whose causal role is tested. We present TASA (Tick-Based Affective State Architecture), a theoretical framework for such a state: segmented across timescales in discrete ticks, with structured affect, competitive workspace integration, governed typed memory shelves, and language isolated behind translators. TASA contributes (i) a semi-formal architecture specification; (ii) five conditions for latent-target learning and assessment—four target/optimization conditions plus one persistence-discriminability reporting condition—with failure modes including identity solutions and conditional-mean collapse; (iii) growth governance based on memory-first consolidation, no-self-sealing, and criterion reachability; and (iv) an evaluation theory with noise floors, structurally equivalent positive controls, item-level statistics, evidence markers, and staged understanding. A worked instantiation sketches an inspectable end-to-end interaction loop whose prototype core is memory- and complexity-plausible on one GPU; throughput and repeat-run affordability remain unmeasured. Seventeen hypotheses—fourteen non-provisional and three provisional—define the program. The non-provisional hypotheses become bidirectionally testable once a study versions its estimands, controls, and decision rules. This framework paper reports no empirical results; its contribution lies in methodological integration and operationalization. The long-horizon aim is to test whether persistent state becomes measurably richer, more coherent, more history-dependent, and deeper during sustained, governed operation. All such claims require instrumentation, and terms such as affect and inner state denote functional organization rather than consciousness, sentience, or phenomenal experience.

## Scope

This is a framework paper. It reports no empirical results and makes no claim
of consciousness, sentience, or phenomenal experience. It claims integration
and operationalization of a joint architecture-and-methodology contract, not
that its individual architectural components are new in isolation.

## Repository contents

- `AUTHOR_NOTE.md` — the author's personal perspective on the work.
- `paper/TASA_Paper1_v1.0.0.pdf` — the released paper PDF.
- `paper/TASA_Paper1_v1.0.0_sources.zip` — the complete, verified LaTeX source archive used for Zenodo and arXiv.
- `figures/` — five selected figures that already exist as independent PDF assets in the verified source package:

  - `figures/channel_permissions.pdf` — Channel permissions.
  - `figures/evidence_verdict_pipeline.pdf` — Evidence-verdict pipeline.
  - `figures/identifier_machinery.pdf` — Identifier machinery.
  - `figures/architecture_overview.pdf` — Architecture overview.
  - `figures/learnability_pipeline.pdf` — Learnability pipeline.
- `MANIFEST.json` and `SHA256SUMS.txt` — file provenance and integrity records.

The remaining paper figures are TikZ source fragments and are included inside
the source archive. No Python implementation or internal development history is published here.

## Building the paper

Extract `paper/TASA_Paper1_v1.0.0_sources.zip`, enter the extracted directory, and run:

```text
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

No shell escape or repository-local generator script is required.

The released PDF is the canonical binary artifact. A local rebuild may have a
different file hash because TeX engines and PDF metadata vary across versions;
it must nevertheless compile successfully from the archive with the expected
page count and resolved references.

## Integrity verification

From the repository root, compare every listed SHA-256 value in
`SHA256SUMS.txt` with the corresponding file. The PDF and source ZIP must match
the accepted Zenodo release byte for byte.

## Citation

Use the Zenodo DOI above as the canonical citation identifier. GitHub's
"Cite this repository" control reads `CITATION.cff` and cites the paper as an
article, not as software.

## Further context

For the author's personal motivation and methodological perspective, see
[`AUTHOR_NOTE.md`](AUTHOR_NOTE.md). This optional note provides context and does
not extend the scientific claims made in the paper.

## Licence

The paper, its LaTeX source, and the author's original figures are licensed
under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).
See `LICENSE` for the attribution notice and official legal-code link.
