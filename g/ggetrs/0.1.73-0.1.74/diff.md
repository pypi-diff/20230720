# Comparing `tmp/ggetrs-0.1.73.tar.gz` & `tmp/ggetrs-0.1.74.tar.gz`

## Comparing `ggetrs-0.1.73.tar` & `ggetrs-0.1.74.tar`

### file list

```diff
@@ -1,183 +1,185 @@
--rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 ggetrs-0.1.73/Cargo.toml
--rw-r--r--   0     1000     1000      223 2023-05-16 17:35:13.000000 ggetrs-0.1.73/.cargo/config.toml
--rw-r--r--   0     1000     1000     2042 2023-05-16 17:35:13.000000 ggetrs-0.1.73/.github/workflows/ci.yml
--rw-r--r--   0     1000     1000      917 2023-05-16 17:35:13.000000 ggetrs-0.1.73/.github/workflows/deploy.yml
--rw-r--r--   0     1000     1000      381 2023-05-16 17:35:13.000000 ggetrs-0.1.73/.gitignore
--rw-r--r--   0     1000     1000    71316 2023-07-11 18:23:12.000000 ggetrs-0.1.73/Cargo.lock
--rw-r--r--   0     1000     1000     1070 2023-05-16 17:35:13.000000 ggetrs-0.1.73/LICENSE
--rw-r--r--   0     1000     1000     4115 2023-05-16 17:35:13.000000 ggetrs-0.1.73/README.md
--rw-r--r--   0     1000     1000      167 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/book.toml
--rw-r--r--   0     1000     1000     1274 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/SUMMARY.md
--rw-r--r--   0     1000     1000      872 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/archs4/correlate.md
--rw-r--r--   0     1000     1000      832 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/archs4/tissue.md
--rw-r--r--   0     1000     1000      347 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/archs4.md
--rw-r--r--   0     1000     1000      540 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/autocomplete.md
--rw-r--r--   0     1000     1000     2848 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/blast.md
--rw-r--r--   0     1000     1000      357 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/bug_reporting.md
--rw-r--r--   0     1000     1000      593 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/chembl/activity.md
--rw-r--r--   0     1000     1000      286 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/chembl.md
--rw-r--r--   0     1000     1000     1700 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/citations.md
--rw-r--r--   0     1000     1000      785 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/contributing.md
--rw-r--r--   0     1000     1000      238 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/disclaimer.md
--rw-r--r--   0     1000     1000     1753 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/enrichr/enrichr.md
--rw-r--r--   0     1000     1000      990 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/enrichr/list.md
--rw-r--r--   0     1000     1000      439 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/enrichr.md
--rw-r--r--   0     1000     1000     1056 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/database.md
--rw-r--r--   0     1000     1000      825 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/lookup-id.md
--rw-r--r--   0     1000     1000      872 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/lookup-symbol.md
--rw-r--r--   0     1000     1000     1567 2023-06-16 19:57:28.000000 ggetrs-0.1.73/docs/src/ensembl/ref.md
--rw-r--r--   0     1000     1000      182 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/release.md
--rw-r--r--   0     1000     1000       75 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/search.md
--rw-r--r--   0     1000     1000     1187 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl/species.md
--rw-r--r--   0     1000     1000      838 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ensembl.md
--rw-r--r--   0     1000     1000     1419 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/faq.md
--rw-r--r--   0     1000     1000      919 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/info.md
--rw-r--r--   0     1000     1000     1288 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/install.md
--rw-r--r--   0     1000     1000     1960 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/introduction.md
--rw-r--r--   0     1000     1000     2364 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/modules.md
--rw-r--r--   0     1000     1000      434 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ncbi/query_ids.md
--rw-r--r--   0     1000     1000      631 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ncbi/query_symbols.md
--rw-r--r--   0     1000     1000      547 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ncbi/taxons.md
--rw-r--r--   0     1000     1000      469 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ncbi.md
--rw-r--r--   0     1000     1000      690 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/pdb/info.md
--rw-r--r--   0     1000     1000      661 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/pdb/structure.md
--rw-r--r--   0     1000     1000      361 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/pdb.md
--rw-r--r--   0     1000     1000     1369 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/search.md
--rw-r--r--   0     1000     1000     1911 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/seq.md
--rw-r--r--   0     1000     1000     1246 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ucsc/blat.md
--rw-r--r--   0     1000     1000      264 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/ucsc.md
--rw-r--r--   0     1000     1000      706 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/uniprot/query.md
--rw-r--r--   0     1000     1000      466 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/src/uniprot.md
--rw-r--r--   0     1000     1000     6010 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/theme/css/variables.css
--rw-r--r--   0     1000     1000     4077 2023-05-16 17:35:13.000000 ggetrs-0.1.73/docs/theme/highlight.css
--rw-r--r--   0     1000     1000     1905 2023-05-16 17:35:13.000000 ggetrs-0.1.73/justfile
--rw-r--r--   0     1000     1000      459 2023-07-11 18:22:21.000000 ggetrs-0.1.73/pyproject.toml
--rw-r--r--   0     1000     1000     1215 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/cli.rs
--rw-r--r--   0     1000     1000     1873 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/functions/correlation.rs
--rw-r--r--   0     1000     1000       87 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/functions/mod.rs
--rw-r--r--   0     1000     1000     1370 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/functions/tissue.rs
--rw-r--r--   0     1000     1000      369 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/mod.rs
--rw-r--r--   0     1000     1000     1294 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/python.rs
--rw-r--r--   0     1000     1000     2750 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/types/correlation.rs
--rw-r--r--   0     1000     1000      155 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/types/mod.rs
--rw-r--r--   0     1000     1000     4071 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/archs4/types/tissue.rs
--rw-r--r--   0     1000     1000      853 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/cli.rs
--rw-r--r--   0     1000     1000     3370 2023-06-16 19:57:28.000000 ggetrs-0.1.73/src/blast/functions/blast.rs
--rw-r--r--   0     1000     1000       98 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/functions/mod.rs
--rw-r--r--   0     1000     1000   118971 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/functions/utils.rs
--rw-r--r--   0     1000     1000       89 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/mod.rs
--rw-r--r--   0     1000     1000     1640 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/python.rs
--rw-r--r--   0     1000     1000     3450 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/types/conf.rs
--rw-r--r--   0     1000     1000      175 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/types/mod.rs
--rw-r--r--   0     1000     1000     4126 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/types/query.rs
--rw-r--r--   0     1000     1000     5336 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/types/result.rs
--rw-r--r--   0     1000     1000      438 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/blast/types/status.rs
--rw-r--r--   0     1000     1000      546 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/cli.rs
--rw-r--r--   0     1000     1000     1087 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/functions/activity.rs
--rw-r--r--   0     1000     1000       42 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/functions/mod.rs
--rw-r--r--   0     1000     1000       80 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/mod.rs
--rw-r--r--   0     1000     1000     1513 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/types/activity.rs
--rw-r--r--   0     1000     1000       50 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/chembl/types/mod.rs
--rw-r--r--   0     1000     1000      936 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/archs4.rs
--rw-r--r--   0     1000     1000      499 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/chembl.rs
--rw-r--r--   0     1000     1000     4639 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/cli.rs
--rw-r--r--   0     1000     1000     1154 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/enrichr.rs
--rw-r--r--   0     1000     1000     3930 2023-06-16 19:57:28.000000 ggetrs-0.1.73/src/cli/ensembl.rs
--rw-r--r--   0     1000     1000      339 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/mod.rs
--rw-r--r--   0     1000     1000     1224 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/ncbi.rs
--rw-r--r--   0     1000     1000     1195 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/pdb.rs
--rw-r--r--   0     1000     1000      658 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/ucsc.rs
--rw-r--r--   0     1000     1000      609 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/cli/uniprot.rs
--rw-r--r--   0     1000     1000      679 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/constants/filesize.rs
--rw-r--r--   0     1000     1000       98 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/constants/mod.rs
--rw-r--r--   0     1000     1000     1741 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/cli.rs
--rw-r--r--   0     1000     1000     1212 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/add_list.rs
--rw-r--r--   0     1000     1000     1173 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/enrich.rs
--rw-r--r--   0     1000     1000      531 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/get_libraries.rs
--rw-r--r--   0     1000     1000      225 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/mod.rs
--rw-r--r--   0     1000     1000     1521 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/shorthand.rs
--rw-r--r--   0     1000     1000     1123 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/functions/view_list.rs
--rw-r--r--   0     1000     1000      344 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/mod.rs
--rw-r--r--   0     1000     1000      497 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/python.rs
--rw-r--r--   0     1000     1000      603 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/types/add_list.rs
--rw-r--r--   0     1000     1000     2688 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/types/enrich.rs
--rw-r--r--   0     1000     1000     3619 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/types/library.rs
--rw-r--r--   0     1000     1000      232 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/types/mod.rs
--rw-r--r--   0     1000     1000      589 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/enrichr/types/view_list.rs
--rw-r--r--   0     1000     1000     5620 2023-06-21 00:19:25.000000 ggetrs-0.1.73/src/ensembl/cli.rs
--rw-r--r--   0     1000     1000       85 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/constants.rs
--rw-r--r--   0     1000     1000     1825 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/database.rs
--rw-r--r--   0     1000     1000     1353 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/list_species.rs
--rw-r--r--   0     1000     1000     1346 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/lookup_id.rs
--rw-r--r--   0     1000     1000     1703 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/lookup_symbol.rs
--rw-r--r--   0     1000     1000      318 2023-06-16 16:53:37.000000 ggetrs-0.1.73/src/ensembl/functions/mod.rs
--rw-r--r--   0     1000     1000     3520 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/reference.rs
--rw-r--r--   0     1000     1000      667 2023-06-16 16:56:08.000000 ggetrs-0.1.73/src/ensembl/functions/release.rs
--rw-r--r--   0     1000     1000     2569 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/functions/search.rs
--rw-r--r--   0     1000     1000      773 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/mod.rs
--rw-r--r--   0     1000     1000     3844 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/python.rs
--rw-r--r--   0     1000     1000      849 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/database.rs
--rw-r--r--   0     1000     1000     1663 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/datatype.rs
--rw-r--r--   0     1000     1000     1569 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/ftpfile.rs
--rw-r--r--   0     1000     1000     1876 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/lookup.rs
--rw-r--r--   0     1000     1000      305 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/mod.rs
--rw-r--r--   0     1000     1000      270 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/releases.rs
--rw-r--r--   0     1000     1000     2804 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ensembl/types/search_results.rs
--rw-r--r--   0     1000     1000      678 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/info/cli.rs
--rw-r--r--   0     1000     1000     1400 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/info/functions.rs
--rw-r--r--   0     1000     1000      156 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/info/mod.rs
--rw-r--r--   0     1000     1000      799 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/info/python.rs
--rw-r--r--   0     1000     1000     4423 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/info/types.rs
--rw-r--r--   0     1000     1000     1409 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/lib.rs
--rw-r--r--   0     1000     1000     7146 2023-06-21 00:19:25.000000 ggetrs-0.1.73/src/main.rs
--rw-r--r--   0     1000     1000     1700 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/cli.rs
--rw-r--r--   0     1000     1000      139 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/functions/mod.rs
--rw-r--r--   0     1000     1000     1346 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/functions/query_ids.rs
--rw-r--r--   0     1000     1000     1679 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/functions/query_symbols.rs
--rw-r--r--   0     1000     1000     1495 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/functions/taxons.rs
--rw-r--r--   0     1000     1000      276 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/mod.rs
--rw-r--r--   0     1000     1000      698 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/types/container.rs
--rw-r--r--   0     1000     1000     2283 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/types/info.rs
--rw-r--r--   0     1000     1000      187 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/types/mod.rs
--rw-r--r--   0     1000     1000      803 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/types/taxons.rs
--rw-r--r--   0     1000     1000     1874 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ncbi/types/transcript.rs
--rw-r--r--   0     1000     1000     1516 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/cli.rs
--rw-r--r--   0     1000     1000       92 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/functions/mod.rs
--rw-r--r--   0     1000     1000     3431 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/functions/resource.rs
--rw-r--r--   0     1000     1000     1998 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/functions/structure.rs
--rw-r--r--   0     1000     1000      101 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/mod.rs
--rw-r--r--   0     1000     1000       90 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/types/mod.rs
--rw-r--r--   0     1000     1000     2914 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/types/resource.rs
--rw-r--r--   0     1000     1000     1270 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/pdb/types/structure.rs
--rw-r--r--   0     1000     1000     1256 2023-06-16 19:57:28.000000 ggetrs-0.1.73/src/seq/cli.rs
--rw-r--r--   0     1000     1000     3888 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/seq/functions.rs
--rw-r--r--   0     1000     1000      177 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/seq/mod.rs
--rw-r--r--   0     1000     1000      988 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/seq/python.rs
--rw-r--r--   0     1000     1000      887 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/seq/types.rs
--rw-r--r--   0     1000     1000      641 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/cli.rs
--rw-r--r--   0     1000     1000     2277 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/functions/blat.rs
--rw-r--r--   0     1000     1000       30 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/functions/mod.rs
--rw-r--r--   0     1000     1000      115 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/mod.rs
--rw-r--r--   0     1000     1000     1413 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/python.rs
--rw-r--r--   0     1000     1000     5598 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/types/blat.rs
--rw-r--r--   0     1000     1000       84 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/types/mod.rs
--rw-r--r--   0     1000     1000      552 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/ucsc/types/seqtype.rs
--rw-r--r--   0     1000     1000      633 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/uniprot/cli.rs
--rw-r--r--   0     1000     1000       33 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/uniprot/functions/mod.rs
--rw-r--r--   0     1000     1000     3003 2023-06-21 00:10:10.000000 ggetrs-0.1.73/src/uniprot/functions/query.rs
--rw-r--r--   0     1000     1000      260 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/uniprot/mod.rs
--rw-r--r--   0     1000     1000       75 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/uniprot/types/mod.rs
--rw-r--r--   0     1000     1000     7982 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/uniprot/types/uniprotinfo.rs
--rw-r--r--   0     1000     1000      216 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/utils/autocomplete.rs
--rw-r--r--   0     1000     1000     1356 2023-06-16 19:57:28.000000 ggetrs-0.1.73/src/utils/download.rs
--rw-r--r--   0     1000     1000     1305 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/utils/fasta.rs
--rw-r--r--   0     1000     1000      175 2023-06-16 19:57:28.000000 ggetrs-0.1.73/src/utils/mod.rs
--rw-r--r--   0     1000     1000     2309 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/utils/parsing.rs
--rw-r--r--   0     1000     1000      674 2023-05-16 17:35:13.000000 ggetrs-0.1.73/src/utils/ping.rs
--rw-r--r--   0     1000     1000      448 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_archs4.py
--rw-r--r--   0     1000     1000      234 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_enrichr.py
--rw-r--r--   0     1000     1000     1991 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_ensembl.py
--rw-r--r--   0     1000     1000      544 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_info.py
--rw-r--r--   0     1000     1000     1260 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_seq.py
--rw-r--r--   0     1000     1000      873 2023-05-16 17:35:13.000000 ggetrs-0.1.73/testing/test_ucsc.py
--rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 ggetrs-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0     1176 1970-01-01 00:00:00.000000 ggetrs-0.1.74/Cargo.toml
+-rw-r--r--   0     1000     1000      223 2023-05-15 18:30:28.000000 ggetrs-0.1.74/.cargo/config.toml
+-rw-r--r--   0     1000     1000     2042 2023-05-15 18:30:28.000000 ggetrs-0.1.74/.github/workflows/ci.yml
+-rw-r--r--   0     1000     1000      917 2023-05-15 18:30:28.000000 ggetrs-0.1.74/.github/workflows/deploy.yml
+-rw-r--r--   0     1000     1000      381 2023-05-15 18:30:28.000000 ggetrs-0.1.74/.gitignore
+-rw-r--r--   0     1000     1000    71386 2023-07-20 21:39:05.000000 ggetrs-0.1.74/Cargo.lock
+-rw-r--r--   0     1000     1000     1070 2023-05-15 18:30:28.000000 ggetrs-0.1.74/LICENSE
+-rw-r--r--   0     1000     1000     4115 2023-05-15 18:30:28.000000 ggetrs-0.1.74/README.md
+-rw-r--r--   0     1000     1000      167 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/book.toml
+-rw-r--r--   0     1000     1000     1274 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/SUMMARY.md
+-rw-r--r--   0     1000     1000      872 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/archs4/correlate.md
+-rw-r--r--   0     1000     1000      832 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/archs4/tissue.md
+-rw-r--r--   0     1000     1000      347 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/archs4.md
+-rw-r--r--   0     1000     1000      540 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/autocomplete.md
+-rw-r--r--   0     1000     1000     2848 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/blast.md
+-rw-r--r--   0     1000     1000      357 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/bug_reporting.md
+-rw-r--r--   0     1000     1000      593 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/chembl/activity.md
+-rw-r--r--   0     1000     1000      286 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/chembl.md
+-rw-r--r--   0     1000     1000     1700 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/citations.md
+-rw-r--r--   0     1000     1000      785 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/contributing.md
+-rw-r--r--   0     1000     1000      238 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/disclaimer.md
+-rw-r--r--   0     1000     1000     1753 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/enrichr/enrichr.md
+-rw-r--r--   0     1000     1000      990 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/enrichr/list.md
+-rw-r--r--   0     1000     1000      439 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/enrichr.md
+-rw-r--r--   0     1000     1000     1056 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/database.md
+-rw-r--r--   0     1000     1000      825 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/lookup-id.md
+-rw-r--r--   0     1000     1000      872 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/lookup-symbol.md
+-rw-r--r--   0     1000     1000     1567 2023-07-05 23:19:39.000000 ggetrs-0.1.74/docs/src/ensembl/ref.md
+-rw-r--r--   0     1000     1000      182 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/release.md
+-rw-r--r--   0     1000     1000       75 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/search.md
+-rw-r--r--   0     1000     1000     1187 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl/species.md
+-rw-r--r--   0     1000     1000      838 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ensembl.md
+-rw-r--r--   0     1000     1000     1419 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/faq.md
+-rw-r--r--   0     1000     1000      919 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/info.md
+-rw-r--r--   0     1000     1000     1288 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/install.md
+-rw-r--r--   0     1000     1000     1960 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/introduction.md
+-rw-r--r--   0     1000     1000     2364 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/modules.md
+-rw-r--r--   0     1000     1000      434 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ncbi/query_ids.md
+-rw-r--r--   0     1000     1000      631 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ncbi/query_symbols.md
+-rw-r--r--   0     1000     1000      547 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ncbi/taxons.md
+-rw-r--r--   0     1000     1000      469 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ncbi.md
+-rw-r--r--   0     1000     1000      690 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/pdb/info.md
+-rw-r--r--   0     1000     1000      661 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/pdb/structure.md
+-rw-r--r--   0     1000     1000      361 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/pdb.md
+-rw-r--r--   0     1000     1000     1369 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/search.md
+-rw-r--r--   0     1000     1000     1911 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/seq.md
+-rw-r--r--   0     1000     1000     1246 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ucsc/blat.md
+-rw-r--r--   0     1000     1000      264 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/ucsc.md
+-rw-r--r--   0     1000     1000      706 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/uniprot/query.md
+-rw-r--r--   0     1000     1000      466 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/src/uniprot.md
+-rw-r--r--   0     1000     1000     6010 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/theme/css/variables.css
+-rw-r--r--   0     1000     1000     4077 2023-05-15 18:30:28.000000 ggetrs-0.1.74/docs/theme/highlight.css
+-rw-r--r--   0     1000     1000     1905 2023-05-15 18:30:28.000000 ggetrs-0.1.74/justfile
+-rw-r--r--   0     1000     1000      459 2023-07-20 21:48:01.000000 ggetrs-0.1.74/pyproject.toml
+-rw-r--r--   0     1000     1000     1215 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/cli.rs
+-rw-r--r--   0     1000     1000     1873 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/functions/correlation.rs
+-rw-r--r--   0     1000     1000       87 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/functions/mod.rs
+-rw-r--r--   0     1000     1000     1370 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/functions/tissue.rs
+-rw-r--r--   0     1000     1000      369 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/mod.rs
+-rw-r--r--   0     1000     1000     1294 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/python.rs
+-rw-r--r--   0     1000     1000     2750 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/types/correlation.rs
+-rw-r--r--   0     1000     1000      155 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/types/mod.rs
+-rw-r--r--   0     1000     1000     4071 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/archs4/types/tissue.rs
+-rw-r--r--   0     1000     1000      853 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/cli.rs
+-rw-r--r--   0     1000     1000     3370 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/blast/functions/blast.rs
+-rw-r--r--   0     1000     1000       98 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/functions/mod.rs
+-rw-r--r--   0     1000     1000   118971 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/functions/utils.rs
+-rw-r--r--   0     1000     1000       89 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/mod.rs
+-rw-r--r--   0     1000     1000     1640 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/python.rs
+-rw-r--r--   0     1000     1000     3450 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/types/conf.rs
+-rw-r--r--   0     1000     1000      175 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/types/mod.rs
+-rw-r--r--   0     1000     1000     4126 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/types/query.rs
+-rw-r--r--   0     1000     1000     5336 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/types/result.rs
+-rw-r--r--   0     1000     1000      438 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/blast/types/status.rs
+-rw-r--r--   0     1000     1000      546 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/cli.rs
+-rw-r--r--   0     1000     1000     1087 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/functions/activity.rs
+-rw-r--r--   0     1000     1000       42 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/functions/mod.rs
+-rw-r--r--   0     1000     1000       80 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/mod.rs
+-rw-r--r--   0     1000     1000     1513 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/types/activity.rs
+-rw-r--r--   0     1000     1000       50 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/chembl/types/mod.rs
+-rw-r--r--   0     1000     1000      936 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/archs4.rs
+-rw-r--r--   0     1000     1000      499 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/chembl.rs
+-rw-r--r--   0     1000     1000     4639 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/cli.rs
+-rw-r--r--   0     1000     1000     1414 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/cli/enrichr.rs
+-rw-r--r--   0     1000     1000     3930 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/cli/ensembl.rs
+-rw-r--r--   0     1000     1000      339 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/mod.rs
+-rw-r--r--   0     1000     1000     1224 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/ncbi.rs
+-rw-r--r--   0     1000     1000     1195 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/pdb.rs
+-rw-r--r--   0     1000     1000      658 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/ucsc.rs
+-rw-r--r--   0     1000     1000      609 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/cli/uniprot.rs
+-rw-r--r--   0     1000     1000      679 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/constants/filesize.rs
+-rw-r--r--   0     1000     1000       98 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/constants/mod.rs
+-rw-r--r--   0     1000     1000     2658 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/cli.rs
+-rw-r--r--   0     1000     1000     1114 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/functions/add_background.rs
+-rw-r--r--   0     1000     1000     1740 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/functions/add_list.rs
+-rw-r--r--   0     1000     1000     3179 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/functions/enrich.rs
+-rw-r--r--   0     1000     1000      531 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/enrichr/functions/get_libraries.rs
+-rw-r--r--   0     1000     1000      422 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/functions/mod.rs
+-rw-r--r--   0     1000     1000     1521 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/enrichr/functions/shorthand.rs
+-rw-r--r--   0     1000     1000     2065 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/functions/view_list.rs
+-rw-r--r--   0     1000     1000      373 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/mod.rs
+-rw-r--r--   0     1000     1000     2372 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/python.rs
+-rw-r--r--   0     1000     1000      596 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/types/add_background.rs
+-rw-r--r--   0     1000     1000      603 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/enrichr/types/add_list.rs
+-rw-r--r--   0     1000     1000     2688 2023-07-20 21:21:04.000000 ggetrs-0.1.74/src/enrichr/types/enrich.rs
+-rw-r--r--   0     1000     1000     3619 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/enrichr/types/library.rs
+-rw-r--r--   0     1000     1000      299 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/enrichr/types/mod.rs
+-rw-r--r--   0     1000     1000      589 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/enrichr/types/view_list.rs
+-rw-r--r--   0     1000     1000     5620 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/ensembl/cli.rs
+-rw-r--r--   0     1000     1000       85 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/ensembl/constants.rs
+-rw-r--r--   0     1000     1000     1825 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/database.rs
+-rw-r--r--   0     1000     1000     1353 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/list_species.rs
+-rw-r--r--   0     1000     1000     1346 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/lookup_id.rs
+-rw-r--r--   0     1000     1000     1703 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/lookup_symbol.rs
+-rw-r--r--   0     1000     1000      318 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/mod.rs
+-rw-r--r--   0     1000     1000     3520 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/reference.rs
+-rw-r--r--   0     1000     1000      667 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/release.rs
+-rw-r--r--   0     1000     1000     2569 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/functions/search.rs
+-rw-r--r--   0     1000     1000      773 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/mod.rs
+-rw-r--r--   0     1000     1000     3844 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/python.rs
+-rw-r--r--   0     1000     1000      849 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/database.rs
+-rw-r--r--   0     1000     1000     1663 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/datatype.rs
+-rw-r--r--   0     1000     1000     1569 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/ftpfile.rs
+-rw-r--r--   0     1000     1000     1876 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/lookup.rs
+-rw-r--r--   0     1000     1000      305 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/mod.rs
+-rw-r--r--   0     1000     1000      270 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/releases.rs
+-rw-r--r--   0     1000     1000     2804 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ensembl/types/search_results.rs
+-rw-r--r--   0     1000     1000      678 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/info/cli.rs
+-rw-r--r--   0     1000     1000     1400 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/info/functions.rs
+-rw-r--r--   0     1000     1000      156 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/info/mod.rs
+-rw-r--r--   0     1000     1000      799 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/info/python.rs
+-rw-r--r--   0     1000     1000     4423 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/info/types.rs
+-rw-r--r--   0     1000     1000     1520 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/lib.rs
+-rw-r--r--   0     1000     1000     7186 2023-07-20 21:48:01.000000 ggetrs-0.1.74/src/main.rs
+-rw-r--r--   0     1000     1000     1700 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/cli.rs
+-rw-r--r--   0     1000     1000      139 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/functions/mod.rs
+-rw-r--r--   0     1000     1000     1346 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/functions/query_ids.rs
+-rw-r--r--   0     1000     1000     1679 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/functions/query_symbols.rs
+-rw-r--r--   0     1000     1000     1495 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/functions/taxons.rs
+-rw-r--r--   0     1000     1000      276 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/mod.rs
+-rw-r--r--   0     1000     1000      698 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/types/container.rs
+-rw-r--r--   0     1000     1000     2283 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/types/info.rs
+-rw-r--r--   0     1000     1000      187 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/types/mod.rs
+-rw-r--r--   0     1000     1000      803 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/types/taxons.rs
+-rw-r--r--   0     1000     1000     1874 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ncbi/types/transcript.rs
+-rw-r--r--   0     1000     1000     1516 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/cli.rs
+-rw-r--r--   0     1000     1000       92 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/functions/mod.rs
+-rw-r--r--   0     1000     1000     3431 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/functions/resource.rs
+-rw-r--r--   0     1000     1000     1998 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/functions/structure.rs
+-rw-r--r--   0     1000     1000      101 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/mod.rs
+-rw-r--r--   0     1000     1000       90 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/types/mod.rs
+-rw-r--r--   0     1000     1000     2914 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/types/resource.rs
+-rw-r--r--   0     1000     1000     1270 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/pdb/types/structure.rs
+-rw-r--r--   0     1000     1000     1256 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/seq/cli.rs
+-rw-r--r--   0     1000     1000     3888 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/seq/functions.rs
+-rw-r--r--   0     1000     1000      177 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/seq/mod.rs
+-rw-r--r--   0     1000     1000      988 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/seq/python.rs
+-rw-r--r--   0     1000     1000      887 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/seq/types.rs
+-rw-r--r--   0     1000     1000      641 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/cli.rs
+-rw-r--r--   0     1000     1000     2277 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/functions/blat.rs
+-rw-r--r--   0     1000     1000       30 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/functions/mod.rs
+-rw-r--r--   0     1000     1000      115 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/mod.rs
+-rw-r--r--   0     1000     1000     1413 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/python.rs
+-rw-r--r--   0     1000     1000     5598 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/types/blat.rs
+-rw-r--r--   0     1000     1000       84 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/types/mod.rs
+-rw-r--r--   0     1000     1000      552 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/ucsc/types/seqtype.rs
+-rw-r--r--   0     1000     1000      633 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/cli.rs
+-rw-r--r--   0     1000     1000       33 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/functions/mod.rs
+-rw-r--r--   0     1000     1000     3003 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/functions/query.rs
+-rw-r--r--   0     1000     1000      260 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/mod.rs
+-rw-r--r--   0     1000     1000       75 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/types/mod.rs
+-rw-r--r--   0     1000     1000     7982 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/uniprot/types/uniprotinfo.rs
+-rw-r--r--   0     1000     1000      216 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/utils/autocomplete.rs
+-rw-r--r--   0     1000     1000     1356 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/utils/download.rs
+-rw-r--r--   0     1000     1000     1305 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/utils/fasta.rs
+-rw-r--r--   0     1000     1000      175 2023-07-05 23:19:39.000000 ggetrs-0.1.74/src/utils/mod.rs
+-rw-r--r--   0     1000     1000     2309 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/utils/parsing.rs
+-rw-r--r--   0     1000     1000      674 2023-05-15 18:30:28.000000 ggetrs-0.1.74/src/utils/ping.rs
+-rw-r--r--   0     1000     1000      448 2023-05-15 18:30:28.000000 ggetrs-0.1.74/testing/test_archs4.py
+-rw-r--r--   0     1000     1000      234 2023-05-15 18:30:28.000000 ggetrs-0.1.74/testing/test_enrichr.py
+-rw-r--r--   0     1000     1000     1991 2023-07-20 21:48:01.000000 ggetrs-0.1.74/testing/test_ensembl.py
+-rw-r--r--   0     1000     1000      544 2023-05-15 18:30:28.000000 ggetrs-0.1.74/testing/test_info.py
+-rw-r--r--   0     1000     1000     1260 2023-05-15 18:30:28.000000 ggetrs-0.1.74/testing/test_seq.py
+-rw-r--r--   0     1000     1000      873 2023-05-15 18:30:28.000000 ggetrs-0.1.74/testing/test_ucsc.py
+-rw-r--r--   0        0        0     4589 1970-01-01 00:00:00.000000 ggetrs-0.1.74/PKG-INFO
```

### Comparing `ggetrs-0.1.73/Cargo.toml` & `ggetrs-0.1.74/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ggetrs"
-version = "0.1.73"
+version = "0.1.74"
 edition = "2021"
 license = "MIT"
 description = "Efficient querying of biological databases from the command line"
 homepage = "https://noamteyssier.github.io/ggetrs/"
 repository = "https://github.com/noamteyssier/ggetrs"
 documentation = "https://docs.rs/ggetrs"
 categories = ["science", "command-line-utilities"]
```

### Comparing `ggetrs-0.1.73/.github/workflows/ci.yml` & `ggetrs-0.1.74/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/.github/workflows/deploy.yml` & `ggetrs-0.1.74/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/Cargo.lock` & `ggetrs-0.1.74/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -37,28 +37,22 @@
 checksum = "ca972c2ea5f742bfce5687b9aef75506a764f61d37f8f649047846a9686ddb66"
 dependencies = [
  "memchr 0.1.11",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.2"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr 2.5.0",
 ]
 
 [[package]]
-name = "android-tzdata"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
-
-[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -116,17 +110,17 @@
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.3"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8868f09ff8cea88b079da74ae569d9b8c62a23c68c746240b704ee6f7525c89c"
+checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -134,17 +128,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.2"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
 
 [[package]]
 name = "bigdecimal"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6773ddc0eafc0e509fb60e48dff7f450f8e674a0686ae8605e8d9901bd5eefa"
 dependencies = [
@@ -163,15 +157,15 @@
  "cexpr",
  "clang-sys",
  "lazy_static 1.4.0",
  "lazycell",
  "peeking_take_while",
  "proc-macro2",
  "quote",
- "regex 1.8.4",
+ "regex 1.8.1",
  "rustc-hash",
  "shlex",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
@@ -248,17 +242,17 @@
 name = "bufstream"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "40e38929add23cdf8a366df9b0e088953150724bcbe5fc330b0d8eb3b328eec8"
 
 [[package]]
 name = "bumpalo"
-version = "3.13.0"
+version = "3.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
 
 [[package]]
 name = "bytecheck"
 version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
 dependencies = [
@@ -319,21 +313,21 @@
 dependencies = [
  "num",
  "time 0.1.45",
 ]
 
 [[package]]
 name = "chrono"
-version = "0.4.26"
+version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
- "android-tzdata",
  "iana-time-zone",
  "js-sys",
+ "num-integer",
  "num-traits",
  "time 0.1.45",
  "wasm-bindgen",
  "winapi 0.3.9",
 ]
 
 [[package]]
@@ -345,62 +339,62 @@
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.4"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80672091db20273a15cf9fdd4e47ed43b5091ec9841bf4c6145c9dfbbcae09ed"
+checksum = "34d21f9bf1b425d2968943631ec91202fe5e837264063503708b83013f8fc938"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.4"
+version = "4.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1458a1df40e1e2afebb7ab60ce55c1fa8f431146205aa5f4887e0b111c27636"
+checksum = "914c8c79fb560f238ef6429439a30023c862f7a28e688c58f7203f12b29970bd"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_complete"
-version = "4.3.1"
+version = "4.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6b5c519bab3ea61843a7923d074b04245624bb84a64a8c150f5deb014e388b"
+checksum = "1594fe2312ec4abf402076e407628f5c313e54c32ade058521df4ee34ecac8a8"
 dependencies = [
  "clap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.2"
+version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
+checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.5.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
@@ -440,17 +434,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.8"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -493,17 +487,17 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
  "memoffset",
  "scopeguard",
 ]
@@ -516,17 +510,17 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -541,22 +535,22 @@
 name = "derive_utils"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dff8f6a793f528719e1ad4425a52a213ac1214ac7158c5fb97a7f50a64bfc96d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.7"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "encode_unicode"
@@ -633,17 +627,17 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.2.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frunk"
 version = "0.4.1"
@@ -777,15 +771,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -822,38 +816,38 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "ggetrs"
-version = "0.1.73"
+version = "0.1.74"
 dependencies = [
  "anyhow",
  "bitvec",
- "chrono 0.4.26",
+ "chrono 0.4.24",
  "clap",
  "clap_complete",
  "ftp",
  "futures",
  "indicatif",
  "mysql",
  "pyo3",
- "regex 1.8.4",
+ "regex 1.8.1",
  "reqwest",
  "serde",
  "serde-xml-rs",
  "serde_json",
  "tokio",
 ]
 
@@ -990,17 +984,17 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.57"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -1013,17 +1007,17 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.4.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
@@ -1066,22 +1060,22 @@
 [[package]]
 name = "io-enum"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01c662c349c9c9f542e7bfd9134143beb27da4b20dfbc3b3ef5b2a5b507dafbd"
 dependencies = [
  "derive_utils",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.11"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -1106,17 +1100,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "68c16e1bfd491478ab155fd8b4896b86f9ede344949b641e61501e07c2b8b4d5"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kernel32-sys"
 version = "0.2.2"
@@ -1216,17 +1210,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -1243,33 +1237,36 @@
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.8"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.19"
+version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
+dependencies = [
+ "cfg-if",
+]
 
 [[package]]
 name = "lru"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6e8aaa3f231bb4bd57b84b2d5dc3ae7f350265df8aa96492e0bc394a1571909"
 dependencies = [
@@ -1289,17 +1286,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1329,21 +1326,22 @@
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.8"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
+ "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.48.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "mysql"
 version = "23.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f11339ca5c251941805d51362a07823605a80586ced92914ab7de84fba813f"
@@ -1387,25 +1385,25 @@
  "flate2",
  "frunk",
  "lazy_static 1.4.0",
  "lexical",
  "num-bigint",
  "num-traits",
  "rand",
- "regex 1.8.4",
+ "regex 1.8.1",
  "rust_decimal",
  "saturating",
  "serde",
  "serde_json",
  "sha1",
  "sha2",
  "smallvec",
  "subprocess",
  "thiserror",
- "time 0.3.22",
+ "time 0.3.21",
  "uuid",
 ]
 
 [[package]]
 name = "named_pipe"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1508,23 +1506,23 @@
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.54"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1535,28 +1533,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.88"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1568,23 +1566,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
- "windows-targets 0.48.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
@@ -1596,17 +1594,17 @@
 checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
 dependencies = [
  "base64 0.13.1",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.3.0"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
@@ -1647,17 +1645,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "c4ec6d5fe0b140acb27c9a0444118cf55bfbb4e0b259739429abb4521dd67c16"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1736,17 +1734,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1781,14 +1779,23 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
+version = "0.2.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
@@ -1803,51 +1810,51 @@
  "regex-syntax 0.3.9",
  "thread_local",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
- "aho-corasick 1.0.2",
+ "aho-corasick 1.0.1",
  "memchr 2.5.0",
- "regex-syntax 0.7.2",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9ec002c35e86791825ed294b50008eea9ddfc8def4420124fbc6b08db834957"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "rend"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.18"
+version = "0.11.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
+checksum = "13293b639a097af28fc8a90f22add145a9c954e49d77da06263d58cf44d5fb91"
 dependencies = [
- "base64 0.21.2",
+ "base64 0.21.0",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -1903,17 +1910,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust_decimal"
-version = "1.30.0"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0446843641c69436765a35a5a77088e28c2e6a12da93e84aa3ab1cd4aa5a042"
+checksum = "26bd36b60561ee1fb5ec2817f198b6fd09fa571c897a5e86d1487cfc2b096dfc"
 dependencies = [
  "arrayvec",
  "borsh",
  "bytecheck",
  "byteorder",
  "bytes",
  "num-traits",
@@ -1927,17 +1934,17 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -1974,17 +1981,17 @@
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "security-framework"
-version = "2.9.1"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+checksum = "ca2855b3715770894e67cbfa3df957790aa0c9edc3bf06efa1a84d77fa0839d1"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
@@ -1997,17 +2004,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-xml-rs"
 version = "0.6.0"
@@ -2018,28 +2025,28 @@
  "serde",
  "thiserror",
  "xml-rs",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2063,17 +2070,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.7"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -2153,17 +2160,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2176,24 +2183,23 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.6.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
- "autocfg",
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.48.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
@@ -2205,15 +2211,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "thread-id"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9539db560102d1cef46b8b78ce737ff0bb64e7e18d35b2a5688f7d097d0ff03"
@@ -2240,17 +2246,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.22"
+version = "0.3.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
@@ -2280,17 +2286,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -2305,15 +2311,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -2407,17 +2413,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
@@ -2434,17 +2440,17 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "url"
-version = "2.4.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -2457,17 +2463,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.4"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
@@ -2475,18 +2481,19 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "want"
-version = "0.3.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
+checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
 dependencies = [
+ "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2496,77 +2503,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "5b6cb788c4e39112fbe1822277ef6fb3c55cd86b95cb3d3c4c1c9597e4ac74b4"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "35e522ed4105a9d626d885b35d62501b30d9666283a5c8be12c14a8bdafe7822"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.37"
+version = "0.4.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+checksum = "083abe15c5d88556b77bdf7aef403625be9e327ad37c62c4e4129af740168163"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "358a79a0cb89d21db8120cbfb91392335913e4890665b1a7981d9e956903b434"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "4783ce29f09b9d93134d41297aded3a712b7b979e9c6f28c32cb88c973a94869"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.16",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "a901d592cafaa4d711bc324edfaff879ac700b19c3dfd60058d2b445be2691eb"
 
 [[package]]
 name = "wasm-streams"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bbae3363c08332cadccd13b67db371814cd214c2524020932f0804b8cf7c078"
 dependencies = [
@@ -2575,17 +2582,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "16b5f940c7edfdc6d12126d98c9ef4d1b3d470011c47c76a6581df47ad9ba721"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2793,10 +2800,10 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "xml-rs"
-version = "0.8.14"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52839dc911083a8ef63efa4d039d1f58b5e409f923e44c80828f206f66e5541c"
+checksum = "1690519550bfa95525229b9ca2350c63043a4857b3b0013811b2ccf4a2420b01"
```

### Comparing `ggetrs-0.1.73/LICENSE` & `ggetrs-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/README.md` & `ggetrs-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/SUMMARY.md` & `ggetrs-0.1.74/docs/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/archs4/correlate.md` & `ggetrs-0.1.74/docs/src/archs4/correlate.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/archs4/tissue.md` & `ggetrs-0.1.74/docs/src/archs4/tissue.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/autocomplete.md` & `ggetrs-0.1.74/docs/src/autocomplete.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/blast.md` & `ggetrs-0.1.74/docs/src/blast.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/chembl/activity.md` & `ggetrs-0.1.74/docs/src/chembl/activity.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/citations.md` & `ggetrs-0.1.74/docs/src/citations.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/contributing.md` & `ggetrs-0.1.74/docs/src/contributing.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/enrichr/enrichr.md` & `ggetrs-0.1.74/docs/src/enrichr/enrichr.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/enrichr/list.md` & `ggetrs-0.1.74/docs/src/enrichr/list.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl/database.md` & `ggetrs-0.1.74/docs/src/ensembl/database.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl/lookup-id.md` & `ggetrs-0.1.74/docs/src/ensembl/lookup-id.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl/lookup-symbol.md` & `ggetrs-0.1.74/docs/src/ensembl/lookup-symbol.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl/ref.md` & `ggetrs-0.1.74/docs/src/ensembl/ref.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl/species.md` & `ggetrs-0.1.74/docs/src/ensembl/species.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ensembl.md` & `ggetrs-0.1.74/docs/src/ensembl.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/faq.md` & `ggetrs-0.1.74/docs/src/faq.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/info.md` & `ggetrs-0.1.74/docs/src/info.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/install.md` & `ggetrs-0.1.74/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/introduction.md` & `ggetrs-0.1.74/docs/src/introduction.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/modules.md` & `ggetrs-0.1.74/docs/src/modules.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ncbi/query_symbols.md` & `ggetrs-0.1.74/docs/src/ncbi/query_symbols.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ncbi/taxons.md` & `ggetrs-0.1.74/docs/src/ncbi/taxons.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/pdb/info.md` & `ggetrs-0.1.74/docs/src/pdb/info.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/pdb/structure.md` & `ggetrs-0.1.74/docs/src/pdb/structure.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/search.md` & `ggetrs-0.1.74/docs/src/search.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/seq.md` & `ggetrs-0.1.74/docs/src/seq.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/ucsc/blat.md` & `ggetrs-0.1.74/docs/src/ucsc/blat.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/src/uniprot/query.md` & `ggetrs-0.1.74/docs/src/uniprot/query.md`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/theme/css/variables.css` & `ggetrs-0.1.74/docs/theme/css/variables.css`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/docs/theme/highlight.css` & `ggetrs-0.1.74/docs/theme/highlight.css`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/justfile` & `ggetrs-0.1.74/justfile`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/cli.rs` & `ggetrs-0.1.74/src/archs4/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/functions/correlation.rs` & `ggetrs-0.1.74/src/archs4/functions/correlation.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/functions/tissue.rs` & `ggetrs-0.1.74/src/archs4/functions/tissue.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/python.rs` & `ggetrs-0.1.74/src/archs4/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/types/correlation.rs` & `ggetrs-0.1.74/src/archs4/types/correlation.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/archs4/types/tissue.rs` & `ggetrs-0.1.74/src/archs4/types/tissue.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/cli.rs` & `ggetrs-0.1.74/src/blast/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/functions/blast.rs` & `ggetrs-0.1.74/src/blast/functions/blast.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/functions/utils.rs` & `ggetrs-0.1.74/src/blast/functions/utils.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/python.rs` & `ggetrs-0.1.74/src/blast/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/types/conf.rs` & `ggetrs-0.1.74/src/blast/types/conf.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/types/query.rs` & `ggetrs-0.1.74/src/blast/types/query.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/blast/types/result.rs` & `ggetrs-0.1.74/src/blast/types/result.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/chembl/cli.rs` & `ggetrs-0.1.74/src/chembl/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/chembl/functions/activity.rs` & `ggetrs-0.1.74/src/chembl/functions/activity.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/chembl/types/activity.rs` & `ggetrs-0.1.74/src/chembl/types/activity.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/archs4.rs` & `ggetrs-0.1.74/src/cli/archs4.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/cli.rs` & `ggetrs-0.1.74/src/cli/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/enrichr.rs` & `ggetrs-0.1.74/src/cli/enrichr.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 use clap::Subcommand;
 
 #[derive(Subcommand)]
 pub enum ModEnrichr {
+    /// Perform the Enrichr gene set enrichment analysis
     Enrichr {
         /// any database listed at: https://maayanlab.cloud/Enrichr/#libraries
         /// some shorthands include: pathway, transcription, ontology, diseases_drugs, celltypes,
         /// and kinase_interactions.
         #[clap(short, long)]
         library: String,
 
+        /// Optional background gene list to perform enrichment analysis with. Comma delimited
+        #[clap(short, long, value_parser, value_delimiter = ',')]
+        background: Option<Vec<String>>,
+
         /// list of gene symbols to perform enrichment analysis on.
         #[clap(value_parser, required = true)]
         gene_list: Vec<String>,
 
         /// optional filepath to write output to [default=stdout]
         #[clap(short, long)]
         output: Option<String>,
```

### Comparing `ggetrs-0.1.73/src/cli/ensembl.rs` & `ggetrs-0.1.74/src/cli/ensembl.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/ncbi.rs` & `ggetrs-0.1.74/src/cli/ncbi.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/pdb.rs` & `ggetrs-0.1.74/src/cli/pdb.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/ucsc.rs` & `ggetrs-0.1.74/src/cli/ucsc.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/cli/uniprot.rs` & `ggetrs-0.1.74/src/cli/uniprot.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/constants/filesize.rs` & `ggetrs-0.1.74/src/constants/filesize.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/cli.rs` & `ggetrs-0.1.74/src/pdb/cli.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,57 @@
-use std::fs::File;
-use std::io::Write;
-
-use super::{add_list, enrich, get_libraries};
-use reqwest::Result;
-
-/// Main entrypoint to launching the `enrich` function for `Enrichr`
-pub fn launch_enrichr(library: &str, gene_list: &[String], output: &Option<String>) -> Result<()> {
-    let add_list = add_list(gene_list)?;
-    let results = enrich(add_list.user_list_id, library)?;
-    match output {
-        Some(path) => {
-            if let Ok(mut writer) = File::create(path) {
-                writeln!(writer, "{}", results).expect("Unable to write to file");
-            } else {
-                println!("{}", results);
+use super::{
+    functions::{resource_info, structure},
+    types::{PdbFormat, PdbResource},
+};
+use anyhow::Result;
+use std::{fs::File, io::Write};
+
+/// main entrypoint for pdb structure
+pub fn launch_pdb_structure(
+    pdb_id: &str,
+    header_only: bool,
+    format: &PdbFormat,
+    output: &Option<String>,
+) -> Result<()> {
+    let results = structure(pdb_id, header_only, format)?;
+    if let Some(pdb_text) = results {
+        match output {
+            Some(path) => {
+                if let Ok(mut writer) = File::create(path) {
+                    write!(writer, "{}", pdb_text).expect("Unable to write to file");
+                } else {
+                    print!("{}", pdb_text);
+                }
+            }
+            None => {
+                print!("{}", pdb_text);
             }
         }
-        None => {
-            println!("{}", results);
-        }
+    } else {
+        eprintln!("No PDB record found: {}", pdb_id);
     }
     Ok(())
 }
 
-/// Main entrypoint for listing all available libraries in `Enrichr`
-pub fn launch_enrichr_list(
-    minimal: bool,
-    list_categories: bool,
-    category: &Option<usize>,
+/// main entrypoint for pdb resource info
+pub fn launch_pdb_resource(
+    pdb_id: &str,
+    resource: &PdbResource,
+    identifier: &Option<String>,
     output: &Option<String>,
 ) -> Result<()> {
-    let libraries = get_libraries()?;
-
-    let output_str = if list_categories {
-        format!("{}", libraries.categories())
-    } else {
-        let libs = if let Some(cid) = category {
-            libraries.filter_categories(*cid)
-        } else {
-            libraries.libraries()
-        };
-        if minimal {
-            format!("{}", libs.minimal())
-        } else {
-            format!("{}", libs)
-        }
-    };
-
+    let results = resource_info(pdb_id, resource, identifier)?;
+    let repr = serde_json::to_string_pretty(&results)?;
     match output {
         Some(path) => {
             if let Ok(mut writer) = File::create(path) {
-                writeln!(writer, "{}", output_str).expect("Unable to write to file");
+                write!(writer, "{}", repr)?;
             } else {
-                println!("{}", output_str);
+                print!("{}", repr)
             }
         }
         None => {
-            println!("{}", output_str);
+            print!("{}", repr)
         }
     }
-
     Ok(())
 }
```

### Comparing `ggetrs-0.1.73/src/enrichr/functions/add_list.rs` & `ggetrs-0.1.74/src/enrichr/functions/add_list.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
+use super::{ENRICHR_URL, SPEEDRICHR_URL};
 use crate::enrichr::types::ResponseAddList;
 use reqwest::{blocking::Client, Result};
 
 /// Performs a function call to the `addList` API.
-pub fn add_list(gene_list: &[String]) -> Result<ResponseAddList> {
+pub fn add_list(gene_list: &[String], speedrichr: bool) -> Result<ResponseAddList> {
     // defines the web client
     let client = Client::new();
 
     // defines the url (aka the API)
-    let url = "https://maayanlab.cloud/Enrichr/addList";
+    let url = if speedrichr {
+        format!("{}/api/addList", SPEEDRICHR_URL)
+    } else {
+        format!("{}/addList", ENRICHR_URL)
+    };
 
     // join the gene-list with a newline
     let query = gene_list.join("\n");
 
     // basic description
     let description = String::from("rust-gget");
 
     // creates the form for the request
     let form = reqwest::blocking::multipart::Form::new()
-        .text("list", query)
-        .text("description", description);
+        .text("list", query.clone())
+        .text("description", description.clone());
 
     // query the server
     client
         .post(url)
         .multipart(form)
         .send()?
         .json::<ResponseAddList>()
@@ -34,12 +39,23 @@
 
     #[test]
     fn test_add_list() {
         let gene_list = vec!["AP2S1", "NSD1", "LDB1"]
             .iter()
             .map(|x| x.to_string())
             .collect::<Vec<String>>();
-        let response = add_list(&gene_list).unwrap();
+        let response = add_list(&gene_list, false).unwrap();
+        assert!(response.user_list_id > 1);
+        assert!(response.short_id.len() > 1);
+    }
+
+    #[test]
+    fn test_add_list_with_background() {
+        let gene_list = vec!["AP2S1", "NSD1", "LDB1"]
+            .iter()
+            .map(|x| x.to_string())
+            .collect::<Vec<String>>();
+        let response = add_list(&gene_list, true).unwrap();
         assert!(response.user_list_id > 1);
         assert!(response.short_id.len() > 1);
     }
 }
```

### Comparing `ggetrs-0.1.73/src/enrichr/functions/get_libraries.rs` & `ggetrs-0.1.74/src/enrichr/functions/get_libraries.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/functions/shorthand.rs` & `ggetrs-0.1.74/src/enrichr/functions/shorthand.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/types/add_list.rs` & `ggetrs-0.1.74/src/enrichr/types/add_list.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/types/enrich.rs` & `ggetrs-0.1.74/src/enrichr/types/enrich.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/types/library.rs` & `ggetrs-0.1.74/src/enrichr/types/library.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/enrichr/types/view_list.rs` & `ggetrs-0.1.74/src/enrichr/types/view_list.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/cli.rs` & `ggetrs-0.1.74/src/ensembl/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/database.rs` & `ggetrs-0.1.74/src/ensembl/functions/database.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/list_species.rs` & `ggetrs-0.1.74/src/ensembl/functions/list_species.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/lookup_id.rs` & `ggetrs-0.1.74/src/ensembl/functions/lookup_id.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/lookup_symbol.rs` & `ggetrs-0.1.74/src/ensembl/functions/lookup_symbol.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/reference.rs` & `ggetrs-0.1.74/src/ensembl/functions/reference.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/release.rs` & `ggetrs-0.1.74/src/ensembl/functions/release.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/functions/search.rs` & `ggetrs-0.1.74/src/ensembl/functions/search.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/mod.rs` & `ggetrs-0.1.74/src/ensembl/mod.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/python.rs` & `ggetrs-0.1.74/src/ensembl/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/types/database.rs` & `ggetrs-0.1.74/src/ensembl/types/database.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/types/datatype.rs` & `ggetrs-0.1.74/src/ensembl/types/datatype.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/types/ftpfile.rs` & `ggetrs-0.1.74/src/ensembl/types/ftpfile.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/types/lookup.rs` & `ggetrs-0.1.74/src/ensembl/types/lookup.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ensembl/types/search_results.rs` & `ggetrs-0.1.74/src/ensembl/types/search_results.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/info/cli.rs` & `ggetrs-0.1.74/src/info/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/info/functions.rs` & `ggetrs-0.1.74/src/info/functions.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/info/python.rs` & `ggetrs-0.1.74/src/info/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/info/types.rs` & `ggetrs-0.1.74/src/info/types.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/lib.rs` & `ggetrs-0.1.74/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 
 /// Useful generic type for Request Errors
 pub type RequestError = Box<dyn std::error::Error + Send + Sync>;
 
 #[pymodule]
 fn ggetrs(py: Python<'_>, module: &PyModule) -> PyResult<()> {
     module.add_function(wrap_pyfunction!(enrichr::python_enrichr, module)?)?;
+    module.add_function(wrap_pyfunction!(
+        enrichr::python_enrichr_background,
+        module
+    )?)?;
     archs4::python_archs4(py, module)?;
     ensembl::python_ensembl(py, module)?;
     ucsc::python_ucsc(py, module)?;
     module.add_function(wrap_pyfunction!(ensembl::python_ensembl_search, module)?)?;
     module.add_function(wrap_pyfunction!(seq::python_seq, module)?)?;
     module.add_function(wrap_pyfunction!(info::python_info, module)?)?;
     module.add_function(wrap_pyfunction!(blast::python_blast, module)?)?;
```

### Comparing `ggetrs-0.1.73/src/main.rs` & `ggetrs-0.1.74/src/main.rs`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 
 fn main() -> Result<(), RequestError> {
     let cli = Cli::parse();
     match &cli.command {
         Commands::Enrichr(sub) => match sub {
             ModEnrichr::Enrichr {
                 library,
+                background,
                 gene_list,
                 output,
             } => {
-                launch_enrichr(library, gene_list, output)?;
+                launch_enrichr(library, background, gene_list, output)?;
             }
             ModEnrichr::List {
                 minimal,
                 list_categories,
                 category,
                 output,
             } => {
```

### Comparing `ggetrs-0.1.73/src/ncbi/cli.rs` & `ggetrs-0.1.74/src/ncbi/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/functions/query_ids.rs` & `ggetrs-0.1.74/src/ncbi/functions/query_ids.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/functions/query_symbols.rs` & `ggetrs-0.1.74/src/ncbi/functions/query_symbols.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/functions/taxons.rs` & `ggetrs-0.1.74/src/ncbi/functions/taxons.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/types/container.rs` & `ggetrs-0.1.74/src/ncbi/types/container.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/types/info.rs` & `ggetrs-0.1.74/src/ncbi/types/info.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/types/taxons.rs` & `ggetrs-0.1.74/src/ncbi/types/taxons.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ncbi/types/transcript.rs` & `ggetrs-0.1.74/src/ncbi/types/transcript.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/pdb/functions/resource.rs` & `ggetrs-0.1.74/src/pdb/functions/resource.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/pdb/functions/structure.rs` & `ggetrs-0.1.74/src/pdb/functions/structure.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/pdb/types/resource.rs` & `ggetrs-0.1.74/src/pdb/types/resource.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/pdb/types/structure.rs` & `ggetrs-0.1.74/src/pdb/types/structure.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/seq/cli.rs` & `ggetrs-0.1.74/src/seq/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/seq/functions.rs` & `ggetrs-0.1.74/src/seq/functions.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/seq/python.rs` & `ggetrs-0.1.74/src/seq/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/seq/types.rs` & `ggetrs-0.1.74/src/seq/types.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ucsc/cli.rs` & `ggetrs-0.1.74/src/ucsc/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ucsc/functions/blat.rs` & `ggetrs-0.1.74/src/ucsc/functions/blat.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ucsc/python.rs` & `ggetrs-0.1.74/src/ucsc/python.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ucsc/types/blat.rs` & `ggetrs-0.1.74/src/ucsc/types/blat.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/ucsc/types/seqtype.rs` & `ggetrs-0.1.74/src/ucsc/types/seqtype.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/uniprot/cli.rs` & `ggetrs-0.1.74/src/uniprot/cli.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/uniprot/functions/query.rs` & `ggetrs-0.1.74/src/uniprot/functions/query.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/uniprot/types/uniprotinfo.rs` & `ggetrs-0.1.74/src/uniprot/types/uniprotinfo.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/utils/download.rs` & `ggetrs-0.1.74/src/utils/download.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/utils/fasta.rs` & `ggetrs-0.1.74/src/utils/fasta.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/utils/parsing.rs` & `ggetrs-0.1.74/src/utils/parsing.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/src/utils/ping.rs` & `ggetrs-0.1.74/src/utils/ping.rs`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/testing/test_ensembl.py` & `ggetrs-0.1.74/testing/test_ensembl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ggetrs
 import requests
-ENSEMBL_RELEASE = 109
+ENSEMBL_RELEASE = 110
 
 def ping_ensembl_ftp():
     try:
         requests.head("https://ftp.ensembl.org", timeout = 5)
         return True
     except:
         # ensembl ftp server is down; skip check
```

### Comparing `ggetrs-0.1.73/testing/test_info.py` & `ggetrs-0.1.74/testing/test_info.py`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/testing/test_seq.py` & `ggetrs-0.1.74/testing/test_seq.py`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/testing/test_ucsc.py` & `ggetrs-0.1.74/testing/test_ucsc.py`

 * *Files identical despite different names*

### Comparing `ggetrs-0.1.73/PKG-INFO` & `ggetrs-0.1.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggetrs
-Version: 0.1.73
+Version: 0.1.74
 License-File: LICENSE
 Summary: Biological querying and analysis
 Keywords: bioinformatics
 Home-Page: https://noamteyssier.github.io/ggetrs/
 Author-email: Noam Teyssier <noam.teyssier@ucsf.edu>
 License: MIT
 Requires-Python: >=3.8
```

