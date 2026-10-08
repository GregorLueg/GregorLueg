## Heyho

### Who am I...?

Computational biologist working across CRISPR screens, genetics, transcriptomics, multi-omics, clinical data and ontologies. Industry background, mostly pharma and biotech. Spare cycles go into open-source tooling: R packages and Python libraries for computational biology and Rust crates under the hood that make them fast. Firm believer that good science needs performant open-source software that runs without a fat compute bill.

Currently playing with [burn](https://burn.dev) for deep learning and writing GPU kernels via [cubecl](https://github.com/tracel-ai/cubecl).

### Packages

All MIT licensed. R binaries on [R-universe](https://gregorlueg.r-universe.dev/packages) (no Rust compile), Python on PyPI, Rust on crates.io if you want the crates in your own stuff.

<table>
<thead>
<tr><th>R</th><th>Python</th><th>Rust</th><th>Description</th></tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse">bixverse</a><br><a href="https://github.com/GregorLueg/bixverse.plots">bixverse.plots</a></td>
<td></td>
<td><a href="https://github.com/GregorLueg/bixverse-rs">bixverse-rs</a></td>
<td>The kitchen sink. Enrichment, matrix factorisation, gene diffusion and a single cell suite that does a million cells on 16 GB. Plots live in <code>bixverse.plots</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/bixverse.gpu">bixverse.gpu</a></td>
<td></td>
<td></td>
<td>SIMD not enough? GPU kNN, k-means, Harmony, SCENIC, SEACells, Scrublet, sparse PCA and parametric UMAP.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/annsearchR">annsearchR</a></td>
<td><a href="https://github.com/GregorLueg/ann-search-rs/tree/main/python">ann-search</a></td>
<td><a href="https://github.com/GregorLueg/ann-search-rs">ann-search-rs</a></td>
<td>Blazingly fast nearest neighbour search. Loads of indices, quantised variants, GPU via wgpu.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/manifoldsR">manifoldsR</a></td>
<td><a href="https://github.com/GregorLueg/manifolds-rs/tree/main/python">manifolds-rs</a></td>
<td><a href="https://github.com/GregorLueg/manifolds-rs">manifolds-rs</a></td>
<td>UMAP, tSNE, PaCMAP, PHATE, ForceAtlas2 and diffusion maps.</td>
</tr>
<tr>
<td></td>
<td><a href="https://github.com/GregorLueg/evoc-rs/tree/main/python">evoc-rs</a></td>
<td><a href="https://github.com/GregorLueg/evoc-rs">evoc-rs</a></td>
<td>Port of <a href="https://github.com/TutteInstitute/evoc">EVoC</a> clustering. In R via <code>manifoldsR</code>.</td>
</tr>
<tr>
<td><a href="https://github.com/GregorLueg/genewalkR">genewalkR</a></td>
<td></td>
<td><a href="https://github.com/GregorLueg/node2vec-rs">node2vec-rs</a></td>
<td>node2vec and metapath2vec, plus GeneWalk, GeneDrift and other graph methods.</td>
</tr>
<tr>
<td></td>
<td><a href="https://github.com/GregorLueg/bonsai-rs/tree/main/python">bonsai-rs</a></td>
<td><a href="https://github.com/GregorLueg/bonsai-rs">bonsai-rs</a><br><a href="https://github.com/GregorLueg/sanity-sc-rs">sanity-sc-rs</a></td>
<td>Ports of <a href="https://doi.org/10.1038/s41587-026-03220-2">Bonsai</a> and <a href="https://doi.org/10.1038/s41587-021-00875-x">Sanity</a>. Trees where distances hold at every scale.</td>
</tr>
<tr>
<td></td>
<td></td>
<td><a href="https://github.com/GregorLueg/edge-rs">edge-rs</a></td>
<td>edgeR, limma-voom and NEBULA in Rust. NEBULA on the GPU.</td>
</tr>
<tr>
<td></td>
<td></td>
<td><a href="https://github.com/GregorLueg/splatter-sc">splatter-sc</a></td>
<td>CLI version of <a href="https://link.springer.com/article/10.1186/s13059-017-1305-0">splatter</a> for synthetic benchmark data.</td>
</tr>
<tr>
<td></td>
<td></td>
<td><a href="https://github.com/GregorLueg/cubecl-utils-rs">cubecl-utils-rs</a></td>
<td>Shared cubecl kernel helpers across my crates.</td>
</tr>
</tbody>
</table>
