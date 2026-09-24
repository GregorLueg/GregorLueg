## Heyho

### Who am I...?

Computational biologist working across CRISPR screens, genetics, transcriptomics, multi-omics, clinical data and ontologies. Industry background, mostly pharma and biotech. Spare cycles go into open-source tooling: R packages and Python libraries for computational biology and Rust crates that make them fast. Firm believer that good science needs performant open-source software that runs without a fat cloud bill.

Currently playing with [burn](https://burn.dev) for deep learning and writing GPU kernels via [cubecl](https://github.com/tracel-ai/cubecl).

### Packages

All public and MIT licensed. R packages are slowly but surely moving to [R-universe](https://gregorlueg.r-universe.dev/packages)
for easy installations without painful Rust compile times. Python packages are thin wrappers over Rust on PyPI. Rust crates are usable on their own if you want to skip R.

#### Single cell and transcriptomics

<table>
<colgroup>
<col width="150">
<col width="100">
<col width="100">
<col width="100">
<col width="430">
</colgroup>
<thead>
<tr><th width="150">Package</th><th width="100">R-universe</th><th width="100">PyPI</th><th width="100">crates.io</th><th width="430">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse">bixverse</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse"><img src="https://gregorlueg.r-universe.dev/bixverse/badges/version" alt="bixverse R-universe"></a></td>
<td></td>
<td></td>
<td>The kitchen sink. Enrichment (GSEA, GSVA, ssGSEA, Gene Ontology with the ontology baked in), matrix factorisations (ICA, NMF, contrastive PCA), gene diffusion, reciprocal best hits, correlation-based methods, and a single cell suite that scales to a million cells on 16 GB without breaking a sweat.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.gpu">bixverse.gpu</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse.gpu"><img src="https://gregorlueg.r-universe.dev/bixverse.gpu/badges/version" alt="bixverse.gpu R-universe"></a></td>
<td></td>
<td></td>
<td>SIMD not enough? GPU-accelerated kNN, k-means, correlations, Harmony, SCENIC, SEACells, Scrubet and sparse PCA for <code>bixverse</code>. Also powers a parametric UMAP for <code>manifoldsR</code> + GPU-accelerated Adam optimiser for UMAP.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.plots">bixverse.plots</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse.plots"><img src="https://gregorlueg.r-universe.dev/bixverse.plots/badges/version" alt="bixverse.plots R-universe"></a></td>
<td></td>
<td></td>
<td>Plotting sub-package. Covers the single cell workflows in <code>bixverse</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse-rs">bixverse-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/bixverse-rs"><img src="https://img.shields.io/crates/v/bixverse-rs" alt="bixverse-rs crates.io"></a></td>
<td>Core Rust behind <code>bixverse</code>. GPU-accelerated methods, single cell algorithms, most of the heavy lifting.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/sanity-sc-rs">sanity-sc-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/sanity-sc-rs"><img src="https://img.shields.io/crates/v/sanity-sc-rs" alt="sanity-sc-rs crates.io"></a></td>
<td>Clean-room port of <a href="https://doi.org/10.1038/s41587-021-00875-x">Sanity</a>. Raw UMIs in, posterior log expression plus error bars out. CPU and GPU via cubecl. Exists mainly to feed <code>bonsai-rs</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/edge-rs">edge-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/edge-rs"><img src="https://img.shields.io/crates/v/edge-rs" alt="edge-rs crates.io"></a></td>
<td>First attempt at porting edgeR, NEBULA and limma-voom into Rust. Potentially some GPU acceleration coming soon.</td>
</tr>
</tbody>
</table>

#### Embeddings, clustering and trees

<table>
<colgroup>
<col width="150">
<col width="100">
<col width="100">
<col width="100">
<col width="430">
</colgroup>
<thead>
<tr><th width="150">Package</th><th width="100">R-universe</th><th width="100">PyPI</th><th width="100">crates.io</th><th width="430">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/manifoldsR">manifoldsR</a><br><a href="https://github.com/GregorLueg/manifolds-rs">manifolds-rs</a></td>
<td><a href="https://gregorlueg.r-universe.dev/manifoldsR"><img src="https://gregorlueg.r-universe.dev/manifoldsR/badges/version" alt="manifoldsR R-universe"></a></td>
<td><a href="https://pypi.org/project/manifolds-rs/"><img src="https://img.shields.io/pypi/v/manifolds-rs" alt="manifolds-rs PyPI"></a></td>
<td><a href="https://crates.io/crates/manifolds-rs"><img src="https://img.shields.io/crates/v/manifolds-rs" alt="manifolds-rs crates.io"></a></td>
<td>UMAP, tSNE, PaCMAP, diffusion maps and PHATE (CPU) with swappable ANN back-ends from <code>ann-search-rs</code>. Need a very fast UMAP in Python? The wrapper has you covered.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/evoc-rs">evoc-rs</a></td>
<td></td>
<td><a href="https://pypi.org/project/evoc-rs/"><img src="https://img.shields.io/pypi/v/evoc-rs" alt="evoc-rs PyPI"></a></td>
<td><a href="https://crates.io/crates/evoc-rs"><img src="https://img.shields.io/crates/v/evoc-rs" alt="evoc-rs crates.io"></a></td>
<td>Rust port of <a href="https://github.com/TutteInstitute/evoc">EVoC clustering</a> by Leland McInnes. Exposed via <code>manifoldsR</code> since it uses a UMAP-like backbone, and yet another Python wrapper...</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bonsai-rs">bonsai-rs</a></td>
<td></td>
<td><a href="https://pypi.org/project/bonsai-rs/"><img src="https://img.shields.io/pypi/v/bonsai-rs" alt="bonsai-rs PyPI"></a></td>
<td><a href="https://crates.io/crates/bonsai-rs"><img src="https://img.shields.io/crates/v/bonsai-rs" alt="bonsai-rs crates.io"></a></td>
<td>Clean-room port of <a href="https://doi.org/10.1038/s41587-026-03220-2">Bonsai</a>. Tree representations of high-dimensional data where distances hold at every scale, not just locally like UMAP and tSNE. Wants means and error bars, so for scRNA-seq it's raw UMIs, then Sanity, then Bonsai.</td>
</tr>
</tbody>
</table>

#### Nearest neighbour search

<table>
<colgroup>
<col width="150">
<col width="100">
<col width="100">
<col width="100">
<col width="430">
</colgroup>
<thead>
<tr><th width="150">Package</th><th width="100">R-universe</th><th width="100">PyPI</th><th width="100">crates.io</th><th width="430">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/ann-search-rs">ann-search-rs</a></td>
<td></td>
<td><a href="https://pypi.org/project/ann-search/"><img src="https://img.shields.io/pypi/v/ann-search" alt="ann-search PyPI"></a></td>
<td><a href="https://crates.io/crates/ann-search-rs"><img src="https://img.shields.io/crates/v/ann-search-rs" alt="ann-search-rs crates.io"></a></td>
<td>Approximate nearest neighbour search. Highly optimised CPU indices, quantised and binarised variants, plus GPU-accelerated versions. Blazingly fast from Python too.</td>
</tr>
</tbody>
</table>

#### Graphs and networks

<table>
<colgroup>
<col width="150">
<col width="100">
<col width="100">
<col width="100">
<col width="430">
</colgroup>
<thead>
<tr><th width="150">Package</th><th width="100">R-universe</th><th width="100">PyPI</th><th width="100">crates.io</th><th width="430">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/genewalkR">genewalkR</a></td>
<td><a href="https://gregorlueg.r-universe.dev/genewalkR"><img src="https://gregorlueg.r-universe.dev/genewalkR/badges/version" alt="genewalkR R-universe"></a></td>
<td></td>
<td></td>
<td>node2vec interface with a growing collection of graph-heavy computational biology methods: GeneWalk, GeneDrift, random walks and other diffusion approaches.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/node2vec-rs">node2vec-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/node2vec-rs"><img src="https://img.shields.io/crates/v/node2vec-rs" alt="node2vec-rs crates.io"></a></td>
<td>node2vec. Optimised CPU implementation plus a <a href="https://burn.dev">burn</a> version from my first trials with the framework. Also, has now the metapath2vec implementation.</td>
</tr>
</tbody>
</table>

#### GPU plumbing

<table>
<colgroup>
<col width="150">
<col width="100">
<col width="100">
<col width="100">
<col width="430">
</colgroup>
<thead>
<tr><th width="150">Package</th><th width="100">R-universe</th><th width="100">PyPI</th><th width="100">crates.io</th><th width="430">Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/cubecl-utils-rs">cubecl-utils-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/cubecl-utils-rs"><img src="https://img.shields.io/crates/v/cubecl-utils-rs" alt="cubecl-utils-rs crates.io"></a></td>
<td>Shared helpers for cubecl kernels across my crates.</td>
</tr>
</tbody>
</table>
