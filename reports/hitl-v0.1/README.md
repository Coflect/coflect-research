# Coflect HITL Technical Report (arXiv-ready source)

## Files

- `main.tex`: primary report source
- `references.bib`: bibliography

## Build (local)

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

Outputs:

- `main.pdf`

## arXiv submission packaging

Create a clean source archive from this directory:

```bash
tar -czf coflect_hitl_arxiv_v0_1.tar.gz main.tex references.bib
```

Upload the `.tar.gz` to arXiv as source.

## Notes

- The report uses only standard LaTeX packages typically available on arXiv.
- Benchmark numbers in the report are taken from the bundled Coflect benchmark artifact:
  - `docs/benchmarks/hitl_overhead_longrun_2026-03-01.json`
