## Heyho

### Who am I...?

Computational biologist working across CRISPR screens, genetics, transcriptomics, multi-omics, clinical data and ontologies. Industry background, mostly pharma and biotech. Spare cycles go into open-source tooling: R packages and Python libraries for computational biology and Rust crates under the hood that make them fast. Firm believer that good science needs performant open-source software that runs without a fat compute bill.

Currently playing with [burn](https://burn.dev) for deep learning and writing GPU kernels via [cubecl](https://github.com/tracel-ai/cubecl).

### Packages

All MIT licensed. R binaries on [R-universe](https://gregorlueg.r-universe.dev/packages) (no Rust compile), Python on PyPI, Rust on crates.io if you want the crates in your own stuff.

<table>
<thead>
<tr><th>Project</th><th>R</th><th>Python</th><th>Rust</th><th>Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse">bixverse</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2Fbixverse&query=%24.Version&label=bixverse" alt="bixverse"></a><br><a href="https://gregorlueg.r-universe.dev/bixverse.plots"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2Fbixverse.plots&query=%24.Version&label=bixverse.plots" alt="bixverse.plots"></a></td>
<td></td>
<td><a href="https://crates.io/crates/bixverse-rs"><img src="https://img.shields.io/crates/v/bixverse-rs?label=bixverse-rs" alt="bixverse-rs"></a></td>
<td>The kitchen sink. Enrichment, matrix factorisation, gene diffusion and a single cell suite that does a million cells on 16 GB. Plots live in <code>bixverse.plots</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.gpu">bixverse.gpu</a></td>
<td><a href="https://gregorlueg.r-universe.dev/bixverse.gpu"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2Fbixverse.gpu&query=%24.Version&label=bixverse.gpu" alt="bixverse.gpu"></a></td>
<td></td>
<td></td>
<td>SIMD not enough? GPU kNN, k-means, Harmony, SCENIC, SEACells, Scrublet, sparse PCA and parametric UMAP.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/ann-search-rs">ann-search</a></td>
<td><a href="https://gregorlueg.r-universe.dev/annsearchR"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2FannsearchR&query=%24.Version&label=annsearchR" alt="annsearchR"></a></td>
<td><a href="https://pypi.org/project/ann-search/"><img src="https://img.shields.io/pypi/v/ann-search?label=ann-search" alt="ann-search"></a></td>
<td><a href="https://crates.io/crates/ann-search-rs"><img src="https://img.shields.io/crates/v/ann-search-rs?label=ann-search-rs" alt="ann-search-rs"></a></td>
<td>Blazingly fast nearest neighbour search. Loads of indices, quantised variants, GPU via wgpu.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/manifolds-rs">manifolds</a></td>
<td><a href="https://gregorlueg.r-universe.dev/manifoldsR"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2FmanifoldsR&query=%24.Version&label=manifoldsR" alt="manifoldsR"></a></td>
<td><a href="https://pypi.org/project/manifolds-rs/"><img src="https://img.shields.io/pypi/v/manifolds-rs?label=manifolds-rs" alt="manifolds-rs"></a></td>
<td><a href="https://crates.io/crates/manifolds-rs"><img src="https://img.shields.io/crates/v/manifolds-rs?label=manifolds-rs" alt="manifolds-rs"></a></td>
<td>UMAP, tSNE, PaCMAP, PHATE, ForceAtlas2 and diffusion maps.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/evoc-rs">evoc</a></td>
<td></td>
<td><a href="https://pypi.org/project/evoc-rs/"><img src="https://img.shields.io/pypi/v/evoc-rs?label=evoc-rs" alt="evoc-rs"></a></td>
<td><a href="https://crates.io/crates/evoc-rs"><img src="https://img.shields.io/crates/v/evoc-rs?label=evoc-rs" alt="evoc-rs"></a></td>
<td>Port of <a href="https://github.com/TutteInstitute/evoc">EVoC</a> clustering. In R via <code>manifoldsR</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/genewalkR">genewalk</a></td>
<td><a href="https://gregorlueg.r-universe.dev/genewalkR"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fgregorlueg.r-universe.dev%2Fapi%2Fpackages%2FgenewalkR&query=%24.Version&label=genewalkR" alt="genewalkR"></a></td>
<td></td>
<td><a href="https://crates.io/crates/node2vec-rs"><img src="https://img.shields.io/crates/v/node2vec-rs?label=node2vec-rs" alt="node2vec-rs"></a></td>
<td>node2vec and metapath2vec, plus GeneWalk, GeneDrift and other graph methods.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bonsai-rs">bonsai</a></td>
<td></td>
<td><a href="https://pypi.org/project/bonsai-rs/"><img src="https://img.shields.io/pypi/v/bonsai-rs?label=bonsai-rs" alt="bonsai-rs"></a></td>
<td><a href="https://crates.io/crates/bonsai-rs"><img src="https://img.shields.io/crates/v/bonsai-rs?label=bonsai-rs" alt="bonsai-rs"></a><br><a href="https://crates.io/crates/sanity-sc-rs"><img src="https://img.shields.io/crates/v/sanity-sc-rs?label=sanity-sc-rs" alt="sanity-sc-rs"></a></td>
<td>Ports of <a href="https://doi.org/10.1038/s41587-026-03220-2">Bonsai</a> and <a href="https://doi.org/10.1038/s41587-021-00875-x">Sanity</a>. Trees where distances hold at every scale.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/edge-rs">edge-rs</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/edge-rs"><img src="https://img.shields.io/crates/v/edge-rs?label=edge-rs" alt="edge-rs"></a></td>
<td>edgeR, limma-voom and NEBULA in Rust. NEBULA on the GPU.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/splatter-sc">splatter-sc</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/splatter-sc"><img src="https://img.shields.io/crates/v/splatter-sc?label=splatter-sc" alt="splatter-sc"></a></td>
<td>CLI version of <a href="https://link.springer.com/article/10.1186/s13059-017-1305-0">splatter</a> for synthetic benchmark data.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/cubecl-utils-rs">cubecl-utils</a></td>
<td></td>
<td></td>
<td><a href="https://crates.io/crates/cubecl-utils-rs"><img src="https://img.shields.io/crates/v/cubecl-utils-rs?label=cubecl-utils-rs" alt="cubecl-utils-rs"></a></td>
<td>Shared cubecl kernel helpers across my crates.</td>
</tr>
</tbody>
</table>
