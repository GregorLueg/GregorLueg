## Hi there

### Who am I ... ?

Computational biologist working at the intersection of drug discovery and
large-scale biomedical data, think CRISPR screens, genetics, transcriptomics,
multi-omics. </br>
Lately spending more time building open-source tooling specifically for this
domain: R packages for bioinformatics & computational biology and Rust crates,
often combining the two for performance-critical work. Based in industry with
experience in larger pharma companies and small biotechs, but firm
believer that good science needs performant and accessible software that does
not necessitate fat cloud servers. Some Python packages also in the making
around ETLs of large-scale biomedical data. Keep an eye open... ;-)

### R Packages

Below are R packages I created and maintain on the side as labour of passion and
hand-tailored methods.

| Package | Description |
|---------|-------------|
| [genewalkR](https://github.com/GregorLueg/genewalkR) | node2vec interface from Rust that implements different (light) GNN-based compbio methods |
| [manifoldsR](https://github.com/GregorLueg/manifoldsR) | 2D embedding and manifold learning method (think single cell visualisations) in a single package made blazingly fast |
| [bixverse](https://github.com/GregorLueg/bixverse) | The `tidyverse` equivalent for bioinformatics... Highly accelerated and optimised computational biology methods. With alpha version of highly scalable single cell work (soon to be released in main) |

### Rust Crates

Close to dying my hair blue...
Jokes aside, below are the public Rust crates I have created and maintain. These
power the libraries and packages in the interpreted, dynamically typed
languages, see above.

| Crate | crates.io | Description |
|-------|-----------|-------------|
| [node2vec-rs](https://github.com/GregorLueg/node2vec-rs) | [![crates.io](https://img.shields.io/crates/v/node2vec-rs)](https://crates.io/crates/node2vec-rs) | First trials in Burn... Implements node2vec in Burn, but also highly optimised specialised CPU version written in there. |
| [ann-search-rs](https://github.com/GregorLueg/ann-search-rs) | [![crates.io](https://img.shields.io/crates/v/ann-search-rs)](https://crates.io/crates/ann-search-rs) | Various computational biology application need fast (approximate) nearest neighbour searches and I fell in love with that field/methods... Has highly optimised CPU indices, quantised versions and GPU-accelerated ones. |
| [manifolds-rs](https://github.com/GregorLueg/manifolds-rs) | [![crates.io](https://img.shields.io/crates/v/manifolds-rs)](https://crates.io/crates/manifolds-rs) | Implementations of the 2D embedding learning methods that power the manifoldsR package. |
| [bixverse-rs](https://github.com/GregorLueg/bixverse-rs) | [![crates.io](https://img.shields.io/crates/v/bixverse-rs)](https://crates.io/crates/bixverse-rs) | The Rust code powering the bixverse... Initially part of the bixverse package itself, now abstracted out in its independent and growing crate. Future plans include exposing parts to Python. |
