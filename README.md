## Heyho

### Who am I ... ?

Computational biologist/biomedical data sciensts working at the intersection of
drug discovery and large-scale biomedical data, think CRISPR screens, genetics,
transcriptomics, multi-omics, clinical data and and ontologies. AI has become a
bit of a buzzword, but I do enjoy the application of ML/AI where (from my
perception) useful: vector searches, quantisations, graph-based methods are
honestly just cool. Experimenting with [burn](https://burn.dev) as a Deep
Learning framework that can run on most GPUs. Also writing my own
GPU-accelerated methods via [cubecl](https://github.com/tracel-ai/cubecl).</br>
Lately spending more time building open-source tooling: R packages for
bioinformatics & computational biology and Rust crates, often combining the two
for performance-critical work. My background is in industry with experience in
larger pharma companies and small biotechs, but overall just a firm believer
that good science needs performant and accessible open-source software that does
not necessitate fat cloud servers.

### R Packages

Below are R packages I created and maintain on the side as labour of passion:

| Package | Description |
|---------|-------------|
| [bixverse](https://github.com/GregorLueg/bixverse) | The `tidyverse` equivalent for bioinformatics... Highly accelerated and optimised computational biology methods. Also contains a single cell analysis framework enabling million cell analyses on small compute. |
| [bixverse.gpu](https://github.com/GregorLueg/bixverse.gpu) | SIMD-accelerated CPU code not fast enough? Need more oomph? Contains GPU-accelerated methods (mostly for single cell) for the `bixverse` (and also manifoldsR in form of a parametric UMAP). |
| [bixverse.plots](https://github.com/GregorLueg/bixverse.plots) | Plotting helpers for `bixverse` because codebase is already too large... Now contains a large number of plotting functions for the single cell stuff. |
| [genewalkR](https://github.com/GregorLueg/genewalkR) | All types of more specialised graph-based computational methods; has also an implementation of node2vec and methods based on that small neural network. |
| [manifoldsR](https://github.com/GregorLueg/manifoldsR) | 2D embedding and manifold learning method (think single cell visualisations) in a single package made blazingly fast via Rust. |

### Rust Crates

[Close to dying my hair blue...](https://www.youtube.com/watch?v=TGfQu0bQTKc)
Jokes aside, below are the public Rust crates I have created and maintain. These
power the libraries and packages in the interpreted, dynamically typed
languages, see above. There are here as standalone libraries, so, if you wish
to integrate them into your Rust code, all MIT licensed.

| Crate | crates.io | Description |
|-------|-----------|-------------|
| [node2vec-rs](https://github.com/GregorLueg/node2vec-rs) | [![crates.io](https://img.shields.io/crates/v/node2vec-rs)](https://crates.io/crates/node2vec-rs) | First trials in Burn... Implements node2vec in Burn, but also highly optimised specialised CPU version written in there. |
| [ann-search-rs](https://github.com/GregorLueg/ann-search-rs) | [![crates.io](https://img.shields.io/crates/v/ann-search-rs)](https://crates.io/crates/ann-search-rs) | Various computational biology application need fast (approximate) nearest neighbour searches and I fell in love with that field/methods... Has highly optimised CPU indices, quantised versions and GPU-accelerated ones. |
| [manifolds-rs](https://github.com/GregorLueg/manifolds-rs) | [![crates.io](https://img.shields.io/crates/v/manifolds-rs)](https://crates.io/crates/manifolds-rs) | Implementations of the 2D embedding learning methods that power the manifoldsR package. |
| [bixverse-rs](https://github.com/GregorLueg/bixverse-rs) | [![crates.io](https://img.shields.io/crates/v/bixverse-rs)](https://crates.io/crates/bixverse-rs) | The Rust code powering the bixverse... Initially part of the bixverse package itself, now abstracted out in its independent and growing crate. Future plans include exposing parts to Python. Has now also GPU-acceleration components and is growing more and more. |
| [evoc-rs](https://github.com/GregorLueg/evoc-rs) | [![crates.io](https://img.shields.io/crates/v/evoc-rs)](https://crates.io/crates/evoc-rs) | Rust port of the [EVoC clustering](https://github.com/TutteInstitute/evoc) clustering algorithm from the brilliant Leland McInnes. |
