## Heyho

### Who am I...?

Computational biologist working across CRISPR screens, genetics, transcriptomics, multi-omics, clinical data and ontologies. Industry background, mostly pharma and biotech. Spare cycles go into open-source tooling: R packages and Python libraries for computational biology and Rust crates that make them fast. Firm believer that good science needs performant open-source software that runs without a fat cloud bill.

Currently playing with [burn](https://burn.dev) for deep learning and writing GPU kernels via [cubecl](https://github.com/tracel-ai/cubecl).

### R Packages

Public, MIT licensed, slowly but surely also moving to [R-universe](https://gregorlueg.r-universe.dev/packages)
for easy installations without painful Rust compile times.

| Package | R-universe | Description |
|---------|------------|-------------|
| [bixverse](https://github.com/GregorLueg/bixverse) | [![bixverse status badge](https://gregorlueg.r-universe.dev/bixverse/badges/version)](https://gregorlueg.r-universe.dev/bixverse) | The kitchen sink. Enrichment (GSEA, GSVA, ssGSEA, Gene Ontology with the ontology baked in), matrix factorisations (ICA, NMF, contrastive PCA), gene diffusion, reciprocal best hits, correlation-based methods, and a single cell suite that scales to a million cells on 16 GB without breaking a sweat. |
| [bixverse.gpu](https://github.com/GregorLueg/bixverse.gpu) | *To be released* | SIMD not enough? GPU-accelerated kNN, k-means, correlations, Harmony, SCENIC, SEACells, Scrubet and sparse PCA for `bixverse`. Also powers a parametric UMAP for `manifoldsR` + GPU-accelerated Adam optimiser for UMAP. |
| [bixverse.plots](https://github.com/GregorLueg/bixverse.plots) | [![bixverse.plots status badge](https://gregorlueg.r-universe.dev/bixverse.plots/badges/version)](https://gregorlueg.r-universe.dev/bixverse.plots) |Plotting sub-package. Covers the single cell workflows in `bixverse`. |
| [genewalkR](https://github.com/GregorLueg/genewalkR) | [![genewalkR status badge](https://gregorlueg.r-universe.dev/genewalkR/badges/version)](https://gregorlueg.r-universe.dev/genewalkR) | node2vec interface with a growing collection of graph-heavy computational biology methods: GeneWalk, GeneDrift, random walks and other diffusion approaches. |
| [manifoldsR](https://github.com/GregorLueg/manifoldsR) | [![manifoldsR status badge](https://gregorlueg.r-universe.dev/manifoldsR/badges/version)](https://gregorlueg.r-universe.dev/manifoldsR) | UMAP, tSNE, PaCMAP, diffusion maps and PHATE (CPU) with swappable ANN back-ends from `ann-search-rs`. |

### Python packages

Thin wrapper over Rust, MIT licensed and on PyPI. These are barebone wrappers around blazingly fast vector searches, 2D embedding methods for visualisations and EVoC clustering.

| Package | PyPI | Description |
|---------|------|-------------|
| [ann-search](https://gregorlueg.github.io/ann-search-rs/) | [![PyPI](https://img.shields.io/pypi/v/ann-search)](https://pypi.org/project/ann-search/) | Python wrappers over `ann-search-rs` - blazingly fast vector/nearest neighbour search with a wide array of indices and methods. |
| [manifolds-rs](https://gregorlueg.github.io/manifolds-rs/) | [![PyPI](https://img.shields.io/pypi/v/manifolds-rs)](https://pypi.org/project/manifolds-rs/) | Python wrappers over, you guessed it, `manifolds-rs`. If you need a very fast UMAP, tSNE or other embeddding in Python. |


### Rust Crates

Public, MIT licensed, usable on their own if you want to skip R.

| Crate | crates.io | Description |
|-------|-----------|-------------|
| [ann-search-rs](https://github.com/GregorLueg/ann-search-rs) | [![crates.io](https://img.shields.io/crates/v/ann-search-rs)](https://crates.io/crates/ann-search-rs) | Approximate nearest neighbour search. Highly optimised CPU indices, quantised and binarised variants, plus GPU-accelerated versions. |
| [bixverse-rs](https://github.com/GregorLueg/bixverse-rs) | [![crates.io](https://img.shields.io/crates/v/bixverse-rs)](https://crates.io/crates/bixverse-rs) | Core Rust behind `bixverse`. GPU-accelerated methods, single cell algorithms, most of the heavy lifting. |
| [manifolds-rs](https://github.com/GregorLueg/manifolds-rs) | [![crates.io](https://img.shields.io/crates/v/manifolds-rs)](https://crates.io/crates/manifolds-rs) | The 2D embedding methods behind `manifoldsR`. |
| [node2vec-rs](https://github.com/GregorLueg/node2vec-rs) | [![crates.io](https://img.shields.io/crates/v/node2vec-rs)](https://crates.io/crates/node2vec-rs) | node2vec. Optimised CPU implementation plus a [burn](https://burn.dev) version from my first trials with the framework. |
| [evoc-rs](https://github.com/GregorLueg/evoc-rs) | [![crates.io](https://img.shields.io/crates/v/evoc-rs)](https://crates.io/crates/evoc-rs) | Rust port of [EVoC clustering](https://github.com/TutteInstitute/evoc) by Leland McInnes. Exposed via `manifoldsR` since it uses a UMAP-like backbone. |
| [cubecl-utils-rs](https://github.com/GregorLueg/cubecl-utils-rs) | [![crates.io](https://img.shields.io/crates/v/cubecl-utils-rs)](https://crates.io/crates/cubecl-utils-rs) | Shared helpers for cubecl kernels across my crates. |
| [edge-rs](https://github.com/GregorLueg/edge-rs) | [![crates.io](https://img.shields.io/crates/v/edge-rs)](https://crates.io/crates/edge-rs) | First attempt at porting edgeR and NEBULA into Rust |
