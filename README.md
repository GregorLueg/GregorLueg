## Heyho

### Who am I...?

Computational biologist working across CRISPR screens, genetics, transcriptomics, multi-omics, clinical data and ontologies. Industry background, mostly pharma and biotech. Spare cycles go into open-source tooling: R packages and Python libraries for computational biology and Rust crates that make them fast. Firm believer that good science needs performant open-source software that runs without a fat cloud bill.

Currently playing with [burn](https://burn.dev) for deep learning and writing GPU kernels via [cubecl](https://github.com/tracel-ai/cubecl).

### R Packages

Public, MIT licensed, slowly but surely also moving to [R-universe](https://gregorlueg.r-universe.dev/packages)
for easy installations without painful Rust compile times.

<table>
<colgroup>
<col width="160">
<col width="140">
<col width="580">
</colgroup>
<thead>
<tr><th width="160">Package</th><th width="140">R-universe</th><th width="580">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse">bixverse</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse"><img src="https://gregorlueg.r-universe.dev/bixverse/badges/version" alt="bixverse status badge"></a></td>
<td>The kitchen sink. Enrichment (GSEA, GSVA, ssGSEA, Gene Ontology with the ontology baked in), matrix factorisations (ICA, NMF, contrastive PCA), gene diffusion, reciprocal best hits, correlation-based methods, and a single cell suite that scales to a million cells on 16 GB without breaking a sweat.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.gpu">bixverse.gpu</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse.gpu"><img src="https://gregorlueg.r-universe.dev/bixverse.gpu/badges/version" alt="bixverse.gpu status badge"></a></td>
<td>SIMD not enough? GPU-accelerated kNN, k-means, correlations, Harmony, SCENIC, SEACells, Scrubet and sparse PCA for <code>bixverse</code>. Also powers a parametric UMAP for <code>manifoldsR</code> + GPU-accelerated Adam optimiser for UMAP.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.plots">bixverse.plots</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse.plots"><img src="https://gregorlueg.r-universe.dev/bixverse.plots/badges/version" alt="bixverse.plots status badge"></a></td>
<td>Plotting sub-package. Covers the single cell workflows in <code>bixverse</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/genewalkR">genewalkR</a></td>
<td><a href="https://gregorlueg.r-universe.dev/genewalkR"><img src="https://gregorlueg.r-universe.dev/genewalkR/badges/version" alt="genewalkR status badge"></a></td>
<td>node2vec interface with a growing collection of graph-heavy computational biology methods: GeneWalk, GeneDrift, random walks and other diffusion approaches.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/manifoldsR">manifoldsR</a></td>
<td><a href="https://gregorlueg.r-universe.dev/manifoldsR"><img src="https://gregorlueg.r-universe.dev/manifoldsR/badges/version" alt="manifoldsR status badge"></a></td>
<td>UMAP, tSNE, PaCMAP, diffusion maps and PHATE (CPU) with swappable ANN back-ends from <code>ann-search-rs</code>.</td>
</tr>
</tbody>
</table>

### Python packages

Thin wrapper over Rust, MIT licensed and on PyPI. These are barebone wrappers around blazingly fast vector searches, 2D embedding methods for visualisations and EVoC clustering.

<table>
<colgroup>
<col width="160">
<col width="140">
<col width="580">
</colgroup>
<thead>
<tr><th width="160">Package</th><th width="140">PyPI</th><th width="580">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://gregorlueg.github.io/ann-search-rs/">ann-search</a></td>
<td><a href="https://pypi.org/project/ann-search/"><img src="https://img.shields.io/pypi/v/ann-search" alt="PyPI"></a></td>
<td>Python wrappers over <code>ann-search-rs</code> - blazingly fast vector/nearest neighbour search with a wide array of indices and methods.</td>
</tr>
<tr>
<td><a href="https://gregorlueg.github.io/manifolds-rs/">manifolds-rs</a></td>
<td><a href="https://pypi.org/project/manifolds-rs/"><img src="https://img.shields.io/pypi/v/manifolds-rs" alt="PyPI"></a></td>
<td>Python wrappers over, you guessed it, <code>manifolds-rs</code>. If you need a very fast UMAP, tSNE or other embeddding in Python.</td>
</tr>
<tr>
<td><a href="https://gregorlueg.github.io/evoc-rs/">evoc-rs</a></td>
<td><a href="https://pypi.org/project/evoc-rs/"><img src="https://img.shields.io/pypi/v/evoc-rs" alt="PyPI"></a></td>
<td>Yet another Python wrapper... This time over EVoC.</td>
</tr>
</tbody>
</table>

### Rust Crates

Public, MIT licensed, usable on their own if you want to skip R.

<table>
<colgroup>
<col width="160">
<col width="140">
<col width="580">
</colgroup>
<thead>
<tr><th width="160">Crate</th><th width="140">crates.io</th><th width="580">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/ann-search-rs">ann-search-rs</a></td>
<td><a href="https://crates.io/crates/ann-search-rs"><img src="https://img.shields.io/crates/v/ann-search-rs" alt="crates.io"></a></td>
<td>Approximate nearest neighbour search. Highly optimised CPU indices, quantised and binarised variants, plus GPU-accelerated versions.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse-rs">bixverse-rs</a></td>
<td><a href="https://crates.io/crates/bixverse-rs"><img src="https://img.shields.io/crates/v/bixverse-rs" alt="crates.io"></a></td>
<td>Core Rust behind <code>bixverse</code>. GPU-accelerated methods, single cell algorithms, most of the heavy lifting.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/manifolds-rs">manifolds-rs</a></td>
<td><a href="https://crates.io/crates/manifolds-rs"><img src="https://img.shields.io/crates/v/manifolds-rs" alt="crates.io"></a></td>
<td>The 2D embedding methods behind <code>manifoldsR</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/node2vec-rs">node2vec-rs</a></td>
<td><a href="https://crates.io/crates/node2vec-rs"><img src="https://img.shields.io/crates/v/node2vec-rs" alt="crates.io"></a></td>
<td>node2vec. Optimised CPU implementation plus a <a href="https://burn.dev">burn</a> version from my first trials with the framework.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/evoc-rs">evoc-rs</a></td>
<td><a href="https://crates.io/crates/evoc-rs"><img src="https://img.shields.io/crates/v/evoc-rs" alt="crates.io"></a></td>
<td>Rust port of <a href="https://github.com/TutteInstitute/evoc">EVoC clustering</a> by Leland McInnes. Exposed via <code>manifoldsR</code> since it uses a UMAP-like backbone.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/cubecl-utils-rs">cubecl-utils-rs</a></td>
<td><a href="https://crates.io/crates/cubecl-utils-rs"><img src="https://img.shields.io/crates/v/cubecl-utils-rs" alt="crates.io"></a></td>
<td>Shared helpers for cubecl kernels across my crates.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/edge-rs">edge-rs</a></td>
<td><a href="https://crates.io/crates/edge-rs"><img src="https://img.shields.io/crates/v/edge-rs" alt="crates.io"></a></td>
<td>First attempt at porting edgeR and NEBULA into Rust</td>
</tr>
</tbody>
</table>
