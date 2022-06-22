OpenPipeline
================

<!-- README.md is generated by running 'quarto render README.qmd' -->

Extensible single cell analysis pipelines for reproducible and
large-scale single cell processing using Viash and Nextflow.

The provided pipelines are built using the [Viash
framework](http://www.viash.io) on top of the nextflow workflow system.
For more information on Nextflow please visit the [Nextflow github
page](https://github.com/nextflow-io/nextflow) and the [Nextflow read
the docs page](https://www.nextflow.io/docs/latest/index.html).

### Getting started

Run `bin/init`.

### List of components

The results below were generated by running
`bin/viash_build; bin/viash_test`.

<div class="cell-output-display">

| Namespace     | Component                                                                    | Tests                                                                         | Maintainer                              | Duration (s) |
|:--------------|:-----------------------------------------------------------------------------|:------------------------------------------------------------------------------|:----------------------------------------|-------------:|
| cluster       | [leiden](src/cluster/leiden/config.vsh.yaml)                                 | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          147 |
| convert       | [from_10xh5_to_h5mu](src/convert/from_10xh5_to_h5mu/config.vsh.yaml)         | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          153 |
| convert       | [from_10xmtx_to_h5mu](src/convert/from_10xmtx_to_h5mu/config.vsh.yaml)       | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          153 |
| convert       | [from_bdrhap_to_h5mu](src/convert/from_bdrhap_to_h5mu/config.vsh.yaml)       | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          127 |
| convert       | [from_csv_to_h5mu](src/convert/from_csv_to_h5mu/config.vsh.yaml)             | ![tests](https://img.shields.io/badge/tests-no%20tests-orange.png)            | Dries De Maeyer                         |          107 |
| convert       | [from_h5ad_to_h5mu](src/convert/from_h5ad_to_h5mu/config.vsh.yaml)           | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          153 |
| convert       | [from_h5mu_to_seurat](src/convert/from_h5mu_to_seurat/config.vsh.yaml)       | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          139 |
| demux         | [cellranger_mkfastq](src/demux/cellranger_mkfastq/config.vsh.yaml)           | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          131 |
| dimred        | [pca](src/dimred/pca/config.vsh.yaml)                                        | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          160 |
| dimred        | [umap](src/dimred/umap/config.vsh.yaml)                                      | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          153 |
| download      | [download_file](src/download/download_file/config.vsh.yaml)                  | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          118 |
| download      | [sync_test_resources](src/download/sync_test_resources/config.vsh.yaml)      | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          121 |
| filter        | [do_filter](src/filter/do_filter/config.vsh.yaml)                            | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          154 |
| filter        | [filter_with_counts](src/filter/filter_with_counts/config.vsh.yaml)          | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          154 |
| filter        | [filter_with_hvg](src/filter/filter_with_hvg/config.vsh.yaml)                | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          153 |
| filter        | [filter_with_scrublet](src/filter/filter_with_scrublet/config.vsh.yaml)      | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          160 |
| interactive   | [run_cellxgene](src/interactive/run_cellxgene/config.vsh.yaml)               | ![tests](https://img.shields.io/badge/tests-no%20tests-orange.png)            |                                         |           83 |
| interactive   | [run_cirrocumulus](src/interactive/run_cirrocumulus/config.vsh.yaml)         | ![tests](https://img.shields.io/badge/tests-no%20tests-orange.png)            |                                         |           85 |
| mapping       | [bd_rhapsody_wta](src/mapping/bd_rhapsody_wta/config.vsh.yaml)               | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          412 |
| mapping       | [cellranger_count](src/mapping/cellranger_count/config.vsh.yaml)             | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          251 |
| mapping       | [cellranger_count_split](src/mapping/cellranger_count_split/config.vsh.yaml) | ![tests](https://img.shields.io/badge/tests-no%20tests-orange.png)            | [rcannood](https://github.com/rcannood) |           78 |
| neighbors     | [find_neighbors](src/neighbors/find_neighbors/config.vsh.yaml)               | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          154 |
| process_10xh5 | [filter_10xh5](src/process_10xh5/filter_10xh5/config.vsh.yaml)               | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          134 |
| report        | [mermaid](src/report/mermaid/config.vsh.yaml)                                | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          127 |
| transfer      | [publish](src/transfer/publish/config.vsh.yaml)                              | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Toni Verbeiren                          |          118 |
| transform     | [log1p](src/transform/log1p/config.vsh.yaml)                                 | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          143 |
| transform     | [normalize_total](src/transform/normalize_total/config.vsh.yaml)             | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | Dries De Maeyer                         |          147 |
| transform     | [regress_out](src/transform/regress_out/config.vsh.yaml)                     | ![tests](https://img.shields.io/badge/tests-1%20out%20of%201-brightgreen.png) | [rcannood](https://github.com/rcannood) |          160 |

</div>
