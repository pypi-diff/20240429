# Comparing `tmp/genvarloader-0.3.1.tar.gz` & `tmp/genvarloader-0.3.2.tar.gz`

## Comparing `genvarloader-0.3.1.tar` & `genvarloader-0.3.2.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 genvarloader-0.3.1/Cargo.toml
--rw-r--r--   0     1111     7010     2200 2024-04-16 16:39:32.000000 genvarloader-0.3.1/.gitignore
--rw-r--r--   0     1111     7010      432 2024-03-15 17:35:16.000000 genvarloader-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0     1111     7010     1066 2024-02-21 06:02:22.000000 genvarloader-0.3.1/LICENSE.txt
--rw-r--r--   0     1111     7010     2490 2024-02-21 06:02:22.000000 genvarloader-0.3.1/README.md
--rw-r--r--   0     1111     7010     2520 2024-04-16 16:39:32.000000 genvarloader-0.3.1/cli.py
--rw-r--r--   0     1111     7010      624 2024-02-21 06:02:22.000000 genvarloader-0.3.1/dev-environment.yml
--rw-r--r--   0     1111     7010      365 2024-02-21 06:02:22.000000 genvarloader-0.3.1/environment.yml
--rw-r--r--   0     1111     7010   159221 2024-04-16 16:39:32.000000 genvarloader-0.3.1/poetry.lock
--rw-r--r--   0     1111     7010      912 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/__init__.py
--rw-r--r--   0     1111     7010     6056 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/bigwig.py
--rw-r--r--   0     1111     7010      974 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/concurrent.py
--rw-r--r--   0     1111     7010    35779 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/__init__.py
--rw-r--r--   0     1111     7010    32628 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/genotypes.py
--rw-r--r--   0     1111     7010     5335 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/intervals.py
--rw-r--r--   0     1111     7010     1679 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/reference.py
--rw-r--r--   0     1111     7010    15054 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/tracks.py
--rw-r--r--   0     1111     7010     2589 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/utils.py
--rw-r--r--   0     1111     7010    12527 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/dataset/write.py
--rw-r--r--   0     1111     7010     8341 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/fasta.py
--rw-r--r--   0     1111     7010      877 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/genvarloader.pyi
--rw-r--r--   0     1111     7010    25831 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/haplotypes.py
--rw-r--r--   0     1111     7010    10153 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/intervals.py
--rw-r--r--   0     1111     7010    48210 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/loader.py
--rw-r--r--   0     1111     7010        0 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/py.typed
--rw-r--r--   0     1111     7010     4215 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/torch.py
--rw-r--r--   0     1111     7010     8437 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/types.py
--rw-r--r--   0     1111     7010    13407 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/utils.py
--rw-r--r--   0     1111     7010    11614 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/__init__.py
--rw-r--r--   0     1111     7010    28477 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/genotypes.py
--rw-r--r--   0     1111     7010    29659 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/variants/records.py
--rw-r--r--   0     1111     7010    10433 2024-04-16 16:39:32.000000 genvarloader-0.3.1/python/genvarloader/zarr.py
--rw-r--r--   0     1111     7010     4206 2024-04-16 16:39:32.000000 genvarloader-0.3.1/src/bigwig.rs
--rw-r--r--   0     1111     7010     1325 2024-04-16 16:39:32.000000 genvarloader-0.3.1/src/lib.rs
--rw-r--r--   0     1111     7010     1697 2024-02-21 06:05:07.000000 genvarloader-0.3.1/tests/data/pgen/sample.ends.gvl.arrow
--rw-r--r--   0     1111     7010     2189 2024-02-21 06:05:07.000000 genvarloader-0.3.1/tests/data/pgen/sample.gvl.arrow
--rw-r--r--   0     1111     7010       63 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.pgen
--rw-r--r--   0     1111     7010       42 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.psam
--rw-r--r--   0     1111     7010     2241 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/pgen/sample.pvar
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa.fai
--rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa
--rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa.fai
--rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa.fai
--rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa
--rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa.fai
--rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa
--rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa.fai
--rw-r--r--   0     1111     7010     1761 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.ends.gvl.arrow
--rw-r--r--   0     1111     7010     1997 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.arrow
--rw-r--r--   0     1111     7010      223 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zarray
--rw-r--r--   0     1111     7010      133 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zattrs
--rw-r--r--   0     1111     7010    81381 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0
--rw-r--r--   0     1111     7010     2890 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf
--rw-r--r--   0     1111     7010     1272 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf.gz
--rw-r--r--   0     1111     7010      189 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf.gz.csi
--rw-r--r--   0     1111     7010     6218 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/generate_ground_truth.py
--rw-r--r--   0     1111     7010      212 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/sample.bed
--rw-r--r--   0     1111     7010     2327 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/data/vcf/sample.vcf
--rw-r--r--   0     1111     7010     2136 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/dataset/genotypes/test_dense2sparse.py
--rw-r--r--   0     1111     7010     1626 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_fasta.py
--rw-r--r--   0     1111     7010     2814 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_fasta_variants.py
--rw-r--r--   0     1111     7010     1625 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_loader.py
--rw-r--r--   0     1111     7010     3102 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/test_max_ends.py
--rw-r--r--   0     1111     7010     5838 2024-02-21 06:02:23.000000 genvarloader-0.3.1/tests/test_pgen.py
--rw-r--r--   0     1111     7010      391 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/test_utils.py
--rw-r--r--   0     1111     7010      633 2024-02-27 06:15:30.000000 genvarloader-0.3.1/tests/test_variants.py
--rw-r--r--   0     1111     7010     3677 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/bench_cpu_gpu.py
--rw-r--r--   0     1111     7010     3484 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/test_i2t_t2i.py
--rw-r--r--   0     1111     7010     1000 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/test_random_nonoverlapping.py
--rw-r--r--   0     1111     7010     2435 2024-04-16 16:39:32.000000 genvarloader-0.3.1/tests/tracks/utils.py
--rw-r--r--   0     1111     7010    35103 2024-04-16 16:39:32.000000 genvarloader-0.3.1/Cargo.lock
--rw-r--r--   0     1111     7010     1797 2024-04-16 16:52:32.000000 genvarloader-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 genvarloader-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 genvarloader-0.3.2/Cargo.toml
+-rw-r--r--   0     1111     7010     2214 2024-04-29 19:03:18.000000 genvarloader-0.3.2/.gitignore
+-rw-r--r--   0     1111     7010      432 2024-03-15 17:35:16.000000 genvarloader-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0     1111     7010     1066 2024-02-21 06:02:22.000000 genvarloader-0.3.2/LICENSE.txt
+-rw-r--r--   0     1111     7010     2490 2024-02-21 06:02:22.000000 genvarloader-0.3.2/README.md
+-rw-r--r--   0     1111     7010      624 2024-02-21 06:02:22.000000 genvarloader-0.3.2/dev-environment.yml
+-rw-r--r--   0     1111     7010      365 2024-02-21 06:02:22.000000 genvarloader-0.3.2/environment.yml
+-rw-r--r--   0     1111     7010   159221 2024-04-29 18:12:28.000000 genvarloader-0.3.2/poetry.lock
+-rw-r--r--   0     1111     7010      912 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/__init__.py
+-rw-r--r--   0     1111     7010     3692 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/__main__.py
+-rw-r--r--   0     1111     7010     6056 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/bigwig.py
+-rw-r--r--   0     1111     7010      974 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/concurrent.py
+-rw-r--r--   0     1111     7010    37145 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/__init__.py
+-rw-r--r--   0     1111     7010    34411 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/genotypes.py
+-rw-r--r--   0     1111     7010     5335 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/intervals.py
+-rw-r--r--   0     1111     7010     1679 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/reference.py
+-rw-r--r--   0     1111     7010    15054 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/dataset/tracks.py
+-rw-r--r--   0     1111     7010     4110 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/utils.py
+-rw-r--r--   0     1111     7010    15815 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/dataset/write.py
+-rw-r--r--   0     1111     7010     8343 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/fasta.py
+-rw-r--r--   0     1111     7010      877 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/genvarloader.pyi
+-rw-r--r--   0     1111     7010    25831 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/haplotypes.py
+-rw-r--r--   0     1111     7010    10153 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/intervals.py
+-rw-r--r--   0     1111     7010    48210 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/loader.py
+-rw-r--r--   0     1111     7010        0 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/py.typed
+-rw-r--r--   0     1111     7010     4215 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/torch.py
+-rw-r--r--   0     1111     7010     8437 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/types.py
+-rw-r--r--   0     1111     7010    13407 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/utils.py
+-rw-r--r--   0     1111     7010     8986 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/__init__.py
+-rw-r--r--   0     1111     7010     9120 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/genotypes.py
+-rw-r--r--   0     1111     7010    30658 2024-04-29 19:03:18.000000 genvarloader-0.3.2/python/genvarloader/variants/records.py
+-rw-r--r--   0     1111     7010    10433 2024-04-29 18:12:28.000000 genvarloader-0.3.2/python/genvarloader/zarr.py
+-rw-r--r--   0     1111     7010     4206 2024-04-29 18:12:28.000000 genvarloader-0.3.2/src/bigwig.rs
+-rw-r--r--   0     1111     7010     1325 2024-04-29 18:12:28.000000 genvarloader-0.3.2/src/lib.rs
+-rw-r--r--   0     1111     7010     1697 2024-02-21 06:05:07.000000 genvarloader-0.3.2/tests/data/pgen/sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     2189 2024-02-21 06:05:07.000000 genvarloader-0.3.2/tests/data/pgen/sample.gvl.arrow
+-rw-r--r--   0     1111     7010       63 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.pgen
+-rw-r--r--   0     1111     7010       42 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.psam
+-rw-r--r--   0     1111     7010     2241 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/pgen/sample.pvar
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       29 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:22.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00001_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       33 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010      108 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00002_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h1.fa.fai
+-rw-r--r--   0     1111     7010       24 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa
+-rw-r--r--   0     1111     7010       23 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr0_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr10_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr11_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr1_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr2_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h1.fa.fai
+-rw-r--r--   0     1111     7010       26 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr3_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr4_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr5_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr6_h2.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h1.fa.fai
+-rw-r--r--   0     1111     7010       28 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa
+-rw-r--r--   0     1111     7010       27 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr7_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr8_h2.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h1.fa.fai
+-rw-r--r--   0     1111     7010       32 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa
+-rw-r--r--   0     1111     7010       31 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/consensus/sample_NA00003_nr9_h2.fa.fai
+-rw-r--r--   0     1111     7010     1761 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.ends.gvl.arrow
+-rw-r--r--   0     1111     7010     1997 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.arrow
+-rw-r--r--   0     1111     7010      223 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zarray
+-rw-r--r--   0     1111     7010      133 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/.zattrs
+-rw-r--r--   0     1111     7010    81381 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0
+-rw-r--r--   0     1111     7010     2890 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf
+-rw-r--r--   0     1111     7010     1272 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz
+-rw-r--r--   0     1111     7010      189 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz.csi
+-rw-r--r--   0     1111     7010     6218 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/generate_ground_truth.py
+-rw-r--r--   0     1111     7010      212 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/sample.bed
+-rw-r--r--   0     1111     7010     2327 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/data/vcf/sample.vcf
+-rw-r--r--   0     1111     7010     2136 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/dataset/genotypes/test_dense2sparse.py
+-rw-r--r--   0     1111     7010     1626 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_fasta.py
+-rw-r--r--   0     1111     7010     2814 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_fasta_variants.py
+-rw-r--r--   0     1111     7010     1625 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_loader.py
+-rw-r--r--   0     1111     7010     3102 2024-04-16 16:39:32.000000 genvarloader-0.3.2/tests/test_max_ends.py
+-rw-r--r--   0     1111     7010     5838 2024-02-21 06:02:23.000000 genvarloader-0.3.2/tests/test_pgen.py
+-rw-r--r--   0     1111     7010      391 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/test_utils.py
+-rw-r--r--   0     1111     7010      633 2024-02-27 06:15:30.000000 genvarloader-0.3.2/tests/test_variants.py
+-rw-r--r--   0     1111     7010     3677 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/bench_cpu_gpu.py
+-rw-r--r--   0     1111     7010     3484 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/test_i2t_t2i.py
+-rw-r--r--   0     1111     7010     1000 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/test_random_nonoverlapping.py
+-rw-r--r--   0     1111     7010     2435 2024-04-29 18:12:28.000000 genvarloader-0.3.2/tests/tracks/utils.py
+-rw-r--r--   0     1111     7010    35103 2024-04-29 18:12:28.000000 genvarloader-0.3.2/Cargo.lock
+-rw-r--r--   0     1111     7010     1778 2024-04-29 19:04:29.000000 genvarloader-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3355 1970-01-01 00:00:00.000000 genvarloader-0.3.2/PKG-INFO
```

### Comparing `genvarloader-0.3.1/.gitignore` & `genvarloader-0.3.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs/
 requirements.txt
 notebooks/
 scripts/
 .ruff_cache/
 .benchmarks/
 .custom_benchmarks/
+benchmarking/
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `genvarloader-0.3.1/LICENSE.txt` & `genvarloader-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/README.md` & `genvarloader-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/dev-environment.yml` & `genvarloader-0.3.2/dev-environment.yml`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/poetry.lock` & `genvarloader-0.3.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/__init__.py` & `genvarloader-0.3.2/python/genvarloader/__init__.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/bigwig.py` & `genvarloader-0.3.2/python/genvarloader/bigwig.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/concurrent.py` & `genvarloader-0.3.2/python/genvarloader/concurrent.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/__init__.py` & `genvarloader-0.3.2/python/genvarloader/dataset/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     genotypes: Optional[SparseGenotypes] = None
     intervals: Optional[Dict[str, RaggedIntervals]] = None
     transform: Optional[Callable] = None
     idx_map: Optional[NDArray[np.intp]] = None
     return_indices: bool = False
 
     @classmethod
-    def open(
+    def _open(
         cls,
         path: Union[str, Path],
         reference: Optional[Union[str, Path]] = None,
     ):
         """Open a dataset from a path. If no reference genome is provided, the dataset can only yield tracks.
 
         Parameters
@@ -195,30 +195,55 @@
         )
 
         logger.info(f"\n{str(dataset)}")
 
         return dataset
 
     @classmethod
-    def open_with_settings(
+    def open(
         cls,
         path: Union[str, Path],
         reference: Optional[Union[str, Path]] = None,
         samples: Optional[Sequence[str]] = None,
         regions: Optional[Union[str, Path, pl.DataFrame]] = None,
         return_sequences: Optional[Literal[False, "reference", "haplotypes"]] = None,
         return_tracks: Optional[Union[Literal[False], str, List[str]]] = None,
-        transform: Optional[Callable] = None,
+        transform: Optional[Union[Literal[False], Callable]] = None,
         seed: Optional[int] = None,
         jitter: Optional[int] = None,
         return_indices: Optional[bool] = None,
     ):
+        """Open a dataset from a path. If no reference genome is provided, the dataset can only yield tracks.
+
+        Parameters
+        ----------
+        path : Union[str, Path]
+            The path to the dataset.
+        reference : Optional[Union[str, Path]], optional
+            The path to the reference genome, by default None
+        samples : Optional[Sequence[str]], optional
+            The samples to subset to, by default None
+        regions : Optional[Union[str, Path, pl.DataFrame]], optional
+            The regions to subset to, by default None
+        return_sequences : Optional[Literal[False, "reference", "haplotypes"]], optional
+            The sequence type to return. Set this to False to disable returning sequences entirely.
+        return_tracks : Optional[Union[Literal[False], str, List[str]]], optional
+            The tracks to return, by default None. Set this to False to disable returning tracks entirely.
+        transform : Optional[Union[Literal[False], Callable]], optional
+            The transform to set, by default None
+        seed : Optional[int], optional
+            The seed to set, by default None
+        jitter : Optional[int], optional
+            The jitter to set, by default None
+        return_indices : Optional[bool], optional
+            Whether to return indices, by default None
+        """
         if return_sequences is False:
             reference = None
-        ds = cls.open(path, reference).with_settings(
+        ds = cls._open(path, reference).with_settings(
             samples=samples,
             regions=regions,
             return_sequences=return_sequences,
             return_tracks=return_tracks,
             transform=transform,
             seed=seed,
             jitter=jitter,
```

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/genotypes.py` & `genvarloader-0.3.2/python/genvarloader/dataset/genotypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Tuple
+from typing import Tuple, cast
 
 import numba as nb
 import numpy as np
 from attrs import define
 from numpy.typing import NDArray
 
 from ..types import ListIdx
 from ..utils import lengths_to_offsets
-from .utils import padded_slice
+from .utils import padded_slice, reduceat_offsets
 
 
 @define
 class DenseGenotypes:
     """Dense genotypes. In this format, genotypes are stored as a special case of a ragged 3D array where
     each sample has the same number of variants, but each region may have a different number of variants.
     Thus, the first variant indices are the same for every sample, and the offsets are readily computed
@@ -66,27 +66,27 @@
             genos = np.concatenate(genos)
         offsets = offsets.cumsum(dtype=np.uint32)
 
         return DenseGenotypes(genos, first_v_idxs, offsets, self.n_samples)
 
 
 @nb.njit(parallel=True, nogil=True, cache=True)
-def first_v_idxs_to_all_v_idxs(first_variant_indices, n_per_region):
+def first_v_idxs_to_all_v_idxs(first_variant_indices: NDArray, n_per_region: NDArray):
     """Convert first variant indices to variant indices."""
     out = np.empty(n_per_region.sum(), dtype=np.int32)
     out_start = np.empty_like(n_per_region)
     out_start[0] = 0
     out_start[1:] = n_per_region[:-1].cumsum()
     for i in nb.prange(len(first_variant_indices)):
-        _f = first_variant_indices[i]
-        _n = n_per_region[i]
-        if _n == 0:
+        f = first_variant_indices[i]
+        n = n_per_region[i]
+        if n == 0:
             continue
-        _o_s = out_start[i]
-        out[_o_s : _o_s + _n] = np.arange(_f, _f + _n, dtype=np.int32)
+        o_s = out_start[i]
+        out[o_s : o_s + n] = np.arange(f, f + n, dtype=np.int32)
     return out
 
 
 @define
 class SparseGenotypes:
     """Sparse genotypes corresponding to distinct regions. In this format, genotypes are stored as a ragged 3D array where each
     sample, ploid, and region may have a different number of variants, since unknown and REF genotypes are not stored. The
@@ -137,14 +137,35 @@
         """Get variant indices for a given sample and region."""
         i = np.ravel_multi_index(
             (region, sample, ploidy), (self.n_regions, self.n_samples, self.ploidy)
         )
         vars = self.variant_idxs[self.offsets[i] : self.offsets[i + 1]]
         return vars
 
+    def concat(*genos: "SparseGenotypes") -> "SparseGenotypes":
+        """Concatenate sparse genotypes."""
+
+        if not all(g.n_samples == genos[0].n_samples for g in genos):
+            raise ValueError("All genotypes must have the same number of samples.")
+        if not all(g.ploidy == genos[0].ploidy for g in genos):
+            raise ValueError("All genotypes must have the same ploidy.")
+
+        total_n_regions = sum(g.n_regions for g in genos)
+        variant_idxs = np.concatenate([g.variant_idxs for g in genos])
+        offsets = lengths_to_offsets(
+            np.concatenate([np.diff(g.offsets) for g in genos])
+        )
+        return SparseGenotypes(
+            variant_idxs=variant_idxs,
+            offsets=offsets,
+            n_regions=total_n_regions,
+            n_samples=genos[0].n_samples,
+            ploidy=genos[0].ploidy,
+        )
+
     @classmethod
     def from_dense(
         cls,
         genos: NDArray[np.int8],
         first_v_idxs: NDArray[np.int32],
         offsets: NDArray[np.int32],
     ):
@@ -195,51 +216,37 @@
         genos : NDArray[np.int8]
             Shape = (sample, ploidy, variants) Genotypes.
         first_v_idxs : NDArray[np.uint32]
             Shape = (regions) First variant index for each region.
         offsets : NDArray[np.uint32]
             Shape = (regions + 1) Offsets into genos.
         ilens : NDArray[np.int32]
-            Shape = (variants) ILEN of all unique variants.
+            Shape = (total_variants) ILEN of all unique variants.
         positions : NDArray[np.int32]
-            Shape = (total_variants) Positions of variants.
+            Shape = (total_variants) Positions of unique variants.
         starts : NDArray[np.int32]
             Shape = (regions) Start of query regions.
         length : int
             Length of the output haplotypes.
         """
         n_regions = len(first_v_idxs)
         n_samples = genos.shape[0]
         ploidy = genos.shape[1]
-        n_per_region = np.diff(offsets)
-        # (v)
-        dense_v_idxs = first_v_idxs_to_all_v_idxs(first_v_idxs, n_per_region)
         # (s p v)
-        spv_ilens = np.where(genos == 1, ilens[dense_v_idxs], 0)
-        # (s p v)
-        cum_ilens = spv_ilens.cumsum(-1)
-        # (s p r)
-        r_ilens = np.add.reduceat(spv_ilens, offsets[:-1], axis=-1)
-        cum_r_ilens = r_ilens.cumsum(-1)
-        # (r)
-        del spv_ilens
-        # (s p v)
-        keep = get_keep_mask_for_length(
+        keep, min_ilens = get_keep_mask_for_length(
             genos,
-            cum_ilens,
-            cum_r_ilens,
             offsets,
             first_v_idxs,
             positions,
+            ilens,
             starts,
             length,
         )
         # (r)
-        max_ends = starts + length - r_ilens.min((0, 1)).clip(max=0)
-        del cum_ilens, cum_r_ilens, r_ilens
+        max_ends: NDArray[np.int32] = starts + length - min_ilens.clip(max=0)
         # tuple s p v
         n_per_rsp = get_n_per_rsp(keep, offsets, n_regions)
         sparse_offsets = lengths_to_offsets(n_per_rsp.ravel(), np.int32)
         variant_idxs = keep_mask_to_rsp_v_idx(
             keep, first_v_idxs, offsets, sparse_offsets, n_regions, n_samples, ploidy
         )
         sparse_genos = cls(
@@ -248,22 +255,63 @@
             n_regions=n_regions,
             n_samples=n_samples,
             ploidy=ploidy,
         )
         return sparse_genos, max_ends
 
 
+def get_haplotype_ilens(
+    genos: NDArray[np.int8],
+    first_v_idxs: NDArray[np.int32],
+    offsets: NDArray[np.int32],
+    ilens: NDArray[np.int32],
+):
+    # (r)
+    n_per_region = np.diff(offsets)
+    # (v)
+    dense_v_idxs = first_v_idxs_to_all_v_idxs(first_v_idxs, n_per_region)
+    # (s p v)
+    spv_ilens = cast(NDArray[np.int32], np.where(genos == 1, ilens[dense_v_idxs], 0))
+    # (s p r)
+    r_ilens = reduceat_offsets(np.add, spv_ilens, offsets, -1)
+    return spv_ilens, r_ilens
+
+
+@nb.njit(parallel=True, nogil=True, cache=True)
+def get_haplotype_region_ilens(
+    genos: NDArray[np.int8],
+    first_v_idxs: NDArray[np.int32],
+    offsets: NDArray[np.int32],
+    ilens: NDArray[np.int32],
+):
+    n_regions = len(first_v_idxs)
+    n_samples = genos.shape[0]
+    ploidy = genos.shape[1]
+    r_ilens = np.empty((n_samples, ploidy, n_regions), np.int32)
+    for r in nb.prange(n_regions):
+        o_s, o_e = offsets[r], offsets[r + 1]
+        n_v = o_e - o_s
+        if n_v == 0:
+            continue
+        fvi = first_v_idxs[r]
+        for s in nb.prange(n_samples):
+            for p in nb.prange(ploidy):
+                r_ilens[s, p, r] = np.where(
+                    genos[s, p, o_s:o_e] == 1, ilens[fvi : fvi + n_v], 0
+                ).sum()
+    return r_ilens
+
+
 @nb.njit(parallel=True, nogil=True, cache=True)
 def get_keep_mask_for_length(
     genos: NDArray[np.int8],
-    cum_ilens: NDArray[np.int32],
-    cum_r_ilens: NDArray[np.int32],
     offsets: NDArray[np.int32],
     first_v_idxs: NDArray[np.int32],
     positions: NDArray[np.int32],
+    ilens: NDArray[np.int32],
     starts: NDArray[np.int32],
     length: int,
 ):
     """Will mark genotypes to keep based on being an ALT allele and being within the length of the haplotype.
 
     Parameters
     ----------
@@ -284,46 +332,50 @@
     length : int
         Length of haplotypes.
     """
     n_samples = genos.shape[0]
     ploidy = genos.shape[1]
     n_regions = len(starts)
     keep = np.empty_like(genos, np.bool_)
-    for s in nb.prange(n_samples):
-        for p in nb.prange(ploidy):
-            for r in nb.prange(n_regions):
-                o_s, o_e = offsets[r], offsets[r + 1]
-                n_variants = o_e - o_s
-                if n_variants == 0:
-                    continue
-                r_start = starts[r]
-                for v in nb.prange(o_s, o_e):
+    min_ilens = np.empty(n_regions, np.int32)
+    for r in nb.prange(n_regions):
+        o_s, o_e = offsets[r], offsets[r + 1]
+        n_variants = o_e - o_s
+        if n_variants == 0:
+            continue
+        r_start = starts[r]
+        for s in nb.prange(n_samples):
+            for p in nb.prange(ploidy):
+                cum_ilen = 0
+                for v in range(o_s, o_e):
                     v_idx = first_v_idxs[r] + v - o_s
                     rel_pos = positions[v_idx] - r_start
-                    cum_ilen = cum_ilens[s, p, v] - cum_r_ilens[s, p, r]
-                    if rel_pos + cum_ilen < length and genos[s, p, v] == 1:
+                    ilen = ilens[v_idx]
+                    if rel_pos + cum_ilen + ilen < length and genos[s, p, v] == 1:
+                        cum_ilen += ilen
                         keep[s, p, v] = True
                     else:
                         keep[s, p, v] = False
-    return keep
+                min_ilens[r] = min(min_ilens[r], cum_ilen)
+    return keep, min_ilens
 
 
 @nb.njit(parallel=True, nogil=True, cache=True)
 def get_n_per_rsp(keep: NDArray[np.bool_], offsets: NDArray[np.int32], n_regions: int):
     n_samples, ploidy, _ = keep.shape
     n_per_rsp = np.empty((n_regions, n_samples, ploidy), np.int32)
     for r in nb.prange(n_regions):
         o_s, o_e = offsets[r], offsets[r + 1]
         for s in nb.prange(n_samples):
             for p in nb.prange(ploidy):
                 n_per_rsp[r, s, p] = keep[s, p, o_s:o_e].sum()
     return n_per_rsp
 
 
-@nb.njit(parallel=False, nogil=True, cache=True)
+@nb.njit(parallel=True, nogil=True, cache=True)
 def keep_mask_to_rsp_v_idx(
     keep: NDArray[np.bool_],  # (s p v)
     first_v_idxs: NDArray[np.int32],  # (r)
     offsets: NDArray[np.int32],  # (r + 1)
     sparse_offsets: NDArray[np.int32],  # (r*s*p + 1)
     n_regions,
     n_samples,
```

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/intervals.py` & `genvarloader-0.3.2/python/genvarloader/dataset/intervals.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/reference.py` & `genvarloader-0.3.2/python/genvarloader/dataset/reference.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/tracks.py` & `genvarloader-0.3.2/python/genvarloader/dataset/tracks.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/utils.py` & `genvarloader-0.3.2/python/genvarloader/dataset/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Sequence, Tuple
 
 import numba as nb
 import numpy as np
 import polars as pl
 from numpy.typing import ArrayLike, NDArray
 
+from ..utils import DTYPE
+
 
 @nb.njit(nogil=True, cache=True)
 def padded_slice(arr: NDArray, start: int, stop: int, pad_val: int):
     pad_left = -min(0, start)
     pad_right = max(0, stop - len(arr))
 
     if pad_left == 0 and pad_right == 0:
@@ -67,30 +69,82 @@
         pl.col("chromStart", "chromEnd").cast(pl.Int64),
     ).select(*cols)
     return bed
 
 
 @nb.njit(nogil=True, cache=True)
 def splits_sum_le_value(arr: NDArray[np.number], max_value: float) -> NDArray[np.intp]:
-    """Split an array into contiguous sections where the sum is less than or equal to a value.
+    """Get index offsets for groups that sum to no more than a value.
+    Note that values greater than the maximum will be kept in their own group.
 
     Parameters
     ----------
     arr : NDArray[np.number]
         Array to split.
     max_value : float
         Maximum value.
 
     Returns
     -------
-    NDArray[np.int32]
+    NDArray[np.intp]
         Split indices.
+
+    Examples
+    --------
+    >>> splits_sum_le_value(np.array([5, 5, 11, 9, 2, 7]), 10)
+    # (5 5) (11) (9) (2 7)
+    array([0, 2, 3, 4, 6])
     """
     indices = [0]
     current_sum = 0
     for idx, value in enumerate(arr):
         current_sum += value
         if current_sum > max_value:
             indices.append(idx)
             current_sum = value
     indices.append(len(arr))
     return np.array(indices, np.intp)
+
+
+def reduceat_offsets(
+    ufunc: np.ufunc, arr: NDArray[DTYPE], offsets: NDArray[np.integer], axis: int = 0
+) -> NDArray[DTYPE]:
+    """Reduce an array at offsets.
+
+    Parameters
+    ----------
+    ufunc : np.ufunc
+        Ufunc.
+    arr : NDArray[np.number]
+        Array to reduce.
+    offsets : NDArray[np.int32]
+        Offsets.
+    axis : int, optional
+        Axis, by default 0.
+
+    Returns
+    -------
+    out_array
+        Reduced array.
+    """
+    n_reductions = len(offsets) - 1
+
+    if axis < 0:
+        axis = arr.ndim + axis
+
+    no_var_idx = np.searchsorted(offsets, offsets[-1])
+
+    # ensure arr and out are aligned and of same dtype to (hopefully) avoid a copy
+    # https://numpy.org/doc/stable/dev/internals.code-explanations.html#reduceat
+    out_arr = np.empty(
+        (*arr.shape[:axis], n_reductions, *arr.shape[axis + 1 :]), arr.dtype
+    )
+    indices = [slice(None)] * arr.ndim
+    indices[axis] = slice(None, no_var_idx)
+    indices = tuple(indices)
+    ufunc.reduceat(arr, offsets[:no_var_idx], axis=axis, out=out_arr[indices])
+
+    identity_indices = [slice(None)] * arr.ndim
+    identity_indices[axis] = slice(no_var_idx, None)
+    identity_indices = tuple(identity_indices)
+    out_arr[identity_indices] = ufunc.identity
+    return out_arr.swapaxes(axis, -1)
```

### Comparing `genvarloader-0.3.1/python/genvarloader/dataset/write.py` & `genvarloader-0.3.2/python/genvarloader/dataset/write.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import gc
 import json
-import re
 import shutil
 from pathlib import Path
-from typing import TYPE_CHECKING, List, Optional, Tuple, Union, cast
+from typing import Dict, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import polars as pl
 from loguru import logger
 from natsort import natsorted
+from numpy.typing import NDArray
 from tqdm.auto import tqdm
 
 from ..bigwig import BigWigs
-from ..utils import normalize_contig_name, read_bedlike, with_length
+from ..utils import lengths_to_offsets, normalize_contig_name, read_bedlike, with_length
 from ..variants import Variants
 from ..variants.genotypes import VCFGenos
-from .genotypes import SparseGenotypes
+from .genotypes import SparseGenotypes, get_haplotype_region_ilens
+from .utils import splits_sum_le_value
+
+INITIAL_END_EXTENSION = 1000
+EXTEND_END_MULTIPLIER = 1.1
 
 
 def write(
     path: Union[str, Path],
     bed: Union[str, Path, pl.DataFrame],
-    vcf: Optional[Union[str, Path]] = None,
+    variants: Optional[Union[str, Path, Variants]] = None,
     bigwigs: Optional[Union[BigWigs, List[BigWigs]]] = None,
     samples: Optional[List[str]] = None,
     length: Optional[int] = None,
     max_jitter: Optional[int] = None,
     overwrite: bool = False,
+    max_mem: int = 4 * 2**30,
 ):
-    if vcf is None and bigwigs is None:
+    if variants is None and bigwigs is None:
         raise ValueError("At least one of `vcf` or `bigwigs` must be provided.")
 
     if isinstance(bigwigs, BigWigs):
         bigwigs = [bigwigs]
 
-    logger.info(f"Writing to {path}")
+    logger.info(f"Writing dataset to {path}")
 
     metadata = {}
     path = Path(path)
     if path.exists() and overwrite:
         logger.info("Found existing GVL store, overwriting.")
         shutil.rmtree(path)
     elif path.exists() and not overwrite:
@@ -48,28 +53,26 @@
     bed, contigs, region_length = prep_bed(bed, length, max_jitter)
     metadata["region_length"] = region_length
     metadata["contigs"] = contigs
     if max_jitter is not None:
         metadata["max_jitter"] = max_jitter
 
     all_samples: List[str] = []
-    if vcf is not None:
-        vcf = Path(vcf)
-        variants = Variants.from_vcf(vcf, use_cache=False)
+    if variants is not None:
+        if isinstance(variants, (str, Path)):
+            variants = Variants.from_file(variants)
 
         if unavailable_contigs := set(contigs) - {
             normalize_contig_name(c, contigs) for c in variants.records.contigs
         }:
             logger.warning(
                 f"Contigs in queries {unavailable_contigs} are not found in the VCF."
             )
 
         all_samples.extend(variants.samples)
-    else:
-        variants = None
 
     if bigwigs is not None:
         unavail = []
         for bw in bigwigs:
             if unavailable_contigs := set(contigs) - set(
                 normalize_contig_name(c, contigs) for c in bw.contigs
             ):
@@ -93,26 +96,23 @@
     samples.sort()
 
     logger.info(f"Using {len(samples)} samples.")
     metadata["samples"] = samples
     metadata["n_samples"] = len(samples)
     metadata["n_regions"] = bed.height
 
-    if vcf is not None:
-        if TYPE_CHECKING:
-            assert variants is not None
-
+    if variants is not None:
         logger.info("Writing genotypes.")
         bed = write_variants(
             path,
             bed,
-            vcf,
             variants,
             region_length,
             samples,
+            max_mem,
         )
         if isinstance(variants.genotypes, VCFGenos):
             variants.genotypes.close()
         metadata["ploidy"] = variants.ploidy
         # free memory
         del variants
         gc.collect()
@@ -165,28 +165,28 @@
 
     return bed, contigs, length
 
 
 def write_regions(path: Path, bed: pl.DataFrame, contigs: List[str]):
     with pl.StringCache():
         pl.Series(contigs, dtype=pl.Categorical)
-        regions = bed.with_columns(pl.col("chrom").cast(pl.Categorical)).with_columns(
-            pl.all().cast(pl.Int32)
-        )
+        regions = bed.with_columns(
+            pl.col("chrom").cast(pl.Categorical).to_physical()
+        ).with_columns(pl.all().cast(pl.Int32))
     regions = regions.to_numpy()
     np.save(path / "regions.npy", regions)
 
 
 def write_variants(
     path: Path,
     bed: pl.DataFrame,
-    vcf: Path,
     variants: Variants,
     region_length: int,
     samples: Optional[List[str]] = None,
+    max_mem: int = 4 * 2**30,
 ):
     if samples is None:
         len(variants.samples)
         sample_idx = None
         _samples = cast(List[str], variants.samples.tolist())
     else:
         _, key_idx, query_idx = np.intersect1d(
@@ -194,127 +194,222 @@
         )
         if missing := (set(samples) - set(variants.samples)):
             raise ValueError(f"Samples {missing} not found in VCF.")
         sample_idx = key_idx[query_idx]
         len(sample_idx)
         _samples = samples
 
-    gvl_arrow = re.sub(r"\.[bv]cf(\.gz)?$", ".gvl.arrow", vcf.name)
-    recs = pl.read_ipc(vcf.parent / gvl_arrow)
-
     out_dir = path / "genotypes"
     out_dir.mkdir(parents=True, exist_ok=True)
 
-    recs.select("POS", "ALT", "ILEN").write_ipc(out_dir / "variants.arrow")
+    pl.DataFrame(
+        {
+            "POS": np.concatenate(list(variants.records.v_starts.values())),
+            "ALT": pl.concat([a.to_polars() for a in variants.records.alt.values()]),
+            "ILEN": np.concatenate(list(variants.records.v_diffs.values())),
+        }
+    ).write_ipc(out_dir / "variants.arrow")
+
+    rel_start_idxs: Dict[str, NDArray[np.int32]] = {}
+    rel_end_idxs: Dict[str, NDArray[np.int32]] = {}
+    chunk_offsets: Dict[str, NDArray[np.intp]] = {}
+    n_chunks = 0
+    for contig, part in bed.partition_by(
+        "chrom", as_dict=True, include_key=False, maintain_order=True
+    ).items():
+        _contig = normalize_contig_name(contig, variants.records.contigs)
+        if _contig is not None:
+            starts = part["chromStart"].to_numpy()
+            ends = starts + region_length + INITIAL_END_EXTENSION
+            rel_s_idxs = variants.records.find_relative_start_idx(_contig, starts)
+            rel_e_idxs = variants.records.find_relative_end_idx(_contig, ends)
+
+            # variants * ploidy * samples * (1 byte per genotype + 4 bytes per ilen)
+            # + 1 region * ploidy * samples * (4 bytes per ilen)
+            n_variants = rel_e_idxs - rel_s_idxs
+            n_regions = len(starts)
+            mem_per_r = (n_variants * 5 + 4) * len(_samples) * variants.ploidy
+            offsets = splits_sum_le_value(mem_per_r, max_mem)
+            rel_start_idxs[contig] = rel_s_idxs
+            rel_end_idxs[contig] = rel_e_idxs
+            chunk_offsets[contig] = offsets
+            n_chunks += len(offsets) - 1
+        else:
+            rel_start_idxs[contig] = np.zeros(part.height, dtype=np.int32)
+            rel_end_idxs[contig] = np.zeros(part.height, dtype=np.int32)
+            chunk_offsets[contig] = np.array([0, part.height], dtype=np.intp)
 
     v_idx_memmap_offsets = 0
     offset_memmap_offsets = 0
     last_offset = 0
     max_ends = np.empty(bed.height, dtype=np.int32)
     last_max_end_idx = 0
-    with tqdm(total=bed["chrom"].n_unique()) as pbar:
+    with tqdm(total=n_chunks) as pbar:
         for contig, part in bed.partition_by(
             "chrom", as_dict=True, include_key=False, maintain_order=True
         ).items():
-            pbar.set_description(
-                f"Reading genotypes for {part.height} regions on {contig}"
-            )
-            starts = part["chromStart"].to_numpy()
-            ends = part["chromEnd"].to_numpy()
-            n_regions = part.height
+            c_offsets = chunk_offsets[contig]
+            for o_s, o_e in zip(c_offsets[:-1], c_offsets[1:]):
+                rel_s_idxs = rel_start_idxs[contig][o_s:o_e]
+                rel_e_idxs = rel_end_idxs[contig][o_s:o_e]
+                starts = part[o_s:o_e, "chromStart"].to_numpy()
+                ends = starts + region_length + INITIAL_END_EXTENSION
+                n_regions = len(rel_s_idxs)
+                pbar.set_description(
+                    f"Reading genotypes for {n_regions} regions on chromosome {contig}"
+                )
 
-            _contig = normalize_contig_name(contig, variants.records.contigs)
-            if _contig is None:
-                genos = SparseGenotypes.empty(n_regions, len(_samples), variants.ploidy)
-            else:
-                multiplier = 2
-                while True:
-                    records = variants.records.vars_in_range(_contig, starts, ends)
-                    # (s p v)
-                    genos = variants.genotypes.read(
-                        _contig,
-                        records.start_idxs,
-                        records.end_idxs,
-                        sample_idx=sample_idx,
-                    )
-                    # (s p v)
-                    ilens = np.where(genos == 1, records.size_diffs, 0)
-                    # (s p r)
-                    ilens = np.add.reduceat(ilens, records.offsets[:-1], axis=-1)
-                    # (s p r)
-                    effective_length = (ends - starts) + ilens
-                    # (s p r)
-                    missing_length = region_length - effective_length
-                    if np.all(missing_length <= 0):
-                        break
-                    # (r)
-                    ends += multiplier * missing_length.max((0, 1))
+                _contig = normalize_contig_name(contig, variants.records.contigs)
 
-                pbar.set_description(
-                    f"Sparsifying genotypes for {part.height} regions on {contig}"
+                genos, chunk_max_ends = read_variants_chunk(
+                    _contig,
+                    starts,
+                    ends,
+                    rel_s_idxs,
+                    rel_e_idxs,
+                    variants,
+                    region_length,
+                    _samples,
+                    sample_idx,
                 )
-                genos, c_max_ends = SparseGenotypes.from_dense_with_length(
-                    genos=genos,
-                    # make indices relative to the contig
-                    first_v_idxs=records.start_idxs
-                    - variants.records.contig_offsets[_contig],
-                    offsets=records.offsets.astype(np.int32),
-                    ilens=variants.records.v_diffs[_contig],
-                    positions=variants.records.v_starts[_contig],
-                    starts=starts,
-                    length=region_length,
+
+                max_ends[last_max_end_idx : last_max_end_idx + n_regions] = (
+                    chunk_max_ends
                 )
-                # make indices absolute
-                genos.variant_idxs += variants.records.contig_offsets[_contig]
-                max_ends[last_max_end_idx : last_max_end_idx + n_regions] = c_max_ends
                 last_max_end_idx += n_regions
 
-            pbar.set_description(
-                f"Writing genotypes for {part.height} regions on {contig}"
-            )
-            out = np.memmap(
-                out_dir / "variant_idxs.npy",
-                dtype=genos.variant_idxs.dtype,
-                mode="w+" if v_idx_memmap_offsets == 0 else "r+",
-                shape=genos.variant_idxs.shape,
-                offset=v_idx_memmap_offsets,
-            )
-            out[:] = genos.variant_idxs[:]
-            out.flush()
-            v_idx_memmap_offsets += out.nbytes
-
-            offsets = genos.offsets
-            offsets += last_offset
-            last_offset = offsets[-1]
-            out = np.memmap(
-                out_dir / "offsets.npy",
-                dtype=offsets.dtype,
-                mode="w+" if offset_memmap_offsets == 0 else "r+",
-                shape=len(offsets) - 1,
-                offset=offset_memmap_offsets,
-            )
-            out[:] = offsets[:-1]
-            out.flush()
-            offset_memmap_offsets += out.nbytes
-            pbar.update()
+                pbar.set_description(
+                    f"Writing genotypes for {n_regions} regions on chromosome {contig}"
+                )
+                (
+                    v_idx_memmap_offsets,
+                    offset_memmap_offsets,
+                    last_offset,
+                ) = write_variants_chunk(
+                    out_dir,
+                    genos,
+                    v_idx_memmap_offsets,
+                    offset_memmap_offsets,
+                    last_offset,
+                )
+                pbar.update()
 
     out = np.memmap(
         out_dir / "offsets.npy",
-        dtype=offsets.dtype,  # type: ignore
+        dtype=np.int32,
         mode="r+",
         shape=1,
         offset=offset_memmap_offsets,
     )
-    out[-1] = offsets[-1]  # type: ignore
+    out[-1] = last_offset
     out.flush()
 
     bed = bed.with_columns(chromEnd=pl.lit(max_ends))
     return bed
 
 
+def read_variants_chunk(
+    contig: Optional[str],
+    starts: NDArray[np.int32],
+    ends: NDArray[np.int32],
+    rel_s_idx: NDArray[np.int32],
+    rel_e_idx: NDArray[np.int32],
+    variants: Variants,
+    region_length: int,
+    samples: List[str],
+    sample_idx: Optional[NDArray[np.intp]],
+):
+    if contig is None:
+        genos = SparseGenotypes.empty(
+            n_regions=len(rel_s_idx), n_samples=len(samples), ploidy=variants.ploidy
+        )
+        chunk_max_ends = ends
+    else:
+        first = True
+        while True:
+            logger.debug(f"region length {ends[0] - starts[0]}")
+            if not first:
+                rel_e_idx = variants.records.find_relative_end_idx(contig, ends)
+            s_idx = variants.records.contig_offsets[contig] + rel_s_idx
+            e_idx = variants.records.contig_offsets[contig] + rel_e_idx
+            # (s p v)
+            logger.debug("read genotypes")
+            genos = variants.genotypes.read(contig, s_idx, e_idx, sample_idx=sample_idx)
+            n_per_region = e_idx - s_idx
+            offsets = lengths_to_offsets(n_per_region)
+
+            logger.debug("get haplotype region ilens")
+            # (s p r)
+            haplotype_ilens = get_haplotype_region_ilens(
+                genos, rel_s_idx, offsets, variants.records.v_diffs[contig]
+            )
+            haplotype_lengths = ends - starts + haplotype_ilens
+            logger.debug(f"average haplotype length {haplotype_lengths.mean()}")
+            # (s p r)
+            missing_length = region_length - haplotype_lengths
+            logger.debug(f"max missing length {missing_length.max()}")
+
+            if np.all(missing_length <= 0):
+                break
+
+            # (r)
+            ends += np.ceil(
+                EXTEND_END_MULTIPLIER * missing_length.max((0, 1)).clip(min=0)
+            ).astype(np.int32)
+
+        logger.debug("sparsify genotypes")
+        genos, chunk_max_ends = SparseGenotypes.from_dense_with_length(
+            genos=genos,
+            first_v_idxs=rel_s_idx,
+            offsets=offsets,
+            ilens=variants.records.v_diffs[contig],
+            positions=variants.records.v_starts[contig],
+            starts=starts,
+            length=region_length,
+        )
+
+        # make indices absolute
+        genos.variant_idxs += variants.records.contig_offsets[contig]
+    return genos, chunk_max_ends
+
+
+def write_variants_chunk(
+    out_dir: Path,
+    genos: SparseGenotypes,
+    v_idx_memmap_offset: int,
+    offsets_memmap_offset: int,
+    last_offset: int,
+):
+    out = np.memmap(
+        out_dir / "variant_idxs.npy",
+        dtype=genos.variant_idxs.dtype,
+        mode="w+" if v_idx_memmap_offset == 0 else "r+",
+        shape=genos.variant_idxs.shape,
+        offset=v_idx_memmap_offset,
+    )
+    out[:] = genos.variant_idxs[:]
+    out.flush()
+    v_idx_memmap_offset += out.nbytes
+
+    offsets = genos.offsets
+    offsets += last_offset
+    last_offset = offsets[-1]
+    out = np.memmap(
+        out_dir / "offsets.npy",
+        dtype=offsets.dtype,
+        mode="w+" if offsets_memmap_offset == 0 else "r+",
+        shape=len(offsets) - 1,
+        offset=offsets_memmap_offset,
+    )
+    out[:] = offsets[:-1]
+    out.flush()
+    offsets_memmap_offset += out.nbytes
+    return v_idx_memmap_offset, offsets_memmap_offset, last_offset
+
+
 def write_bigwigs(
     path: Path, bed: pl.DataFrame, bigwigs: BigWigs, samples: Optional[List[str]]
 ) -> int:
     if samples is None:
         _samples = cast(List[str], bigwigs.samples)
     else:
         if missing := (set(samples) - set(bigwigs.samples)):
```

### Comparing `genvarloader-0.3.1/python/genvarloader/fasta.py` & `genvarloader-0.3.2/python/genvarloader/fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             self.rev_strand_fn = rev_strand_fn  # type: ignore[assignment]
         else:
             assert_never(self.alphabet)
 
         self.contigs = self._get_contig_lengths()
 
         self.handle: Optional[pysam.FastaFile] = None
-        fa_extension = re.compile(r"\.(fa|fna|fasta)(\.gz)?$")
+        fa_extension = re.compile(r"\.(fa|fna|fasta)(\.b?gz)?$")
         self.cache_path = Path(fa_extension.sub(".fa.gvl", str(self.path)))
 
         if not in_memory:
             self.sequences = None
         else:
             if cache:
                 if not self.cache_path.exists():
```

### Comparing `genvarloader-0.3.1/python/genvarloader/genvarloader.pyi` & `genvarloader-0.3.2/python/genvarloader/genvarloader.pyi`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/haplotypes.py` & `genvarloader-0.3.2/python/genvarloader/haplotypes.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/intervals.py` & `genvarloader-0.3.2/python/genvarloader/intervals.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/loader.py` & `genvarloader-0.3.2/python/genvarloader/loader.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/torch.py` & `genvarloader-0.3.2/python/genvarloader/torch.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/types.py` & `genvarloader-0.3.2/python/genvarloader/types.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/utils.py` & `genvarloader-0.3.2/python/genvarloader/utils.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/python/genvarloader/variants/__init__.py` & `genvarloader-0.3.2/python/genvarloader/variants/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
+import polars as pl
 from attrs import define
 from numpy.typing import ArrayLike, NDArray
 
 from ..utils import normalize_contig_name
 from .genotypes import (
     Genotypes,
-    MemmapGenos,
-    NumpyGenos,
     PgenGenos,
     VCFGenos,
-    VIdxGenos,
-    ZarrGenos,
 )
 from .records import Records, VLenAlleles
 
 __all__ = [
     "PgenGenos",
-    "ZarrGenos",
-    "MemmapGenos",
     "VCFGenos",
     "Variants",
     "Records",
 ]
 
 
 @define
@@ -39,34 +34,49 @@
         Shape : (variants). Difference in length between the REF and the ALT alleles.
     ref : VLenAlleles
         Shape: (variants). REF alleles.
     alt : VLenAlleles
         Shape: (variants). ALT alleles.
     genotypes : NDArray[np.int8]
         Shape: (samples, ploid, variants)
-    offsets : NDArray[np.uint32], optional
+    offsets : NDArray[np.int32], optional
         Shape: (regions + 1). Offsets for the index boundaries of each region such
         that variants for region `i` are `positions[offsets[i] : offsets[i+1]]`,
         `size_diffs[offsets[i] : offsets[i+1]]`, ..., etc.
     """
 
     positions: NDArray[np.int32]
     size_diffs: NDArray[np.int32]
     ref: VLenAlleles
     alt: VLenAlleles
     genotypes: NDArray[np.int8]
-    offsets: NDArray[np.uint32]
+    offsets: NDArray[np.int32]
 
 
 @define
 class Variants:
     records: Records
     genotypes: Genotypes
     _sample_idxs: Optional[NDArray[np.intp]] = None
 
+    @classmethod
+    def from_file(cls, path: Union[str, Path, Dict[str, Path]]):
+        if isinstance(path, (str, Path)):
+            path = Path(path)
+            first_path = path
+        elif isinstance(path, dict):
+            first_path = next(iter(path.values()))
+
+        if first_path.suffix == ".vcf":
+            return cls.from_vcf(path)
+        elif first_path.suffix == ".pgen":
+            return cls.from_pgen(path)
+        else:
+            raise ValueError("Unsupported file type.")
+
     @property
     def chunked(self):
         return self.genotypes.chunked
 
     @property
     def samples(self):
         if self._sample_idxs is None:
@@ -80,20 +90,15 @@
         return len(self._sample_idxs)
 
     @property
     def ploidy(self):
         return self.genotypes.ploidy
 
     @classmethod
-    def from_vcf(
-        cls,
-        vcf: Union[str, Path, Dict[str, Path]],
-        use_cache: bool = True,
-        chunk_shape: Optional[Tuple[int, int, int]] = None,
-    ):
+    def from_vcf(cls, vcf: Union[str, Path, Dict[str, Path]]):
         """Currently does not support multi-allelic sites, but does support *split*
         multi-allelic sites. Note that SVs and "other" variants are also not supported.
         VCFs can be prepared by running:
         ```bash
         bcftools view -i 'TYPE="snp" || TYPE="indel"' <file.bcf> \\
         | bcftools norm \\
             -a \\
@@ -102,48 +107,19 @@
             -f <ref.fa> \\
             -O b \\
             -o <norm.bcf>
         ```
         """
         records = Records.from_vcf(vcf)
 
-        if use_cache:
-            try:
-                genotypes = ZarrGenos(vcf)
-            except FileNotFoundError:
-                genotypes = VCFGenos(vcf, records.contig_offsets)
-                genotypes = ZarrGenos.from_recs_genos(
-                    records, genotypes, chunk_shape=chunk_shape
-                )
-        else:
-            genotypes = VCFGenos(vcf, records.contig_offsets)
-        return cls(records, genotypes)
-
-    @classmethod
-    def from_gvl(cls, path: Union[str, Path, Dict[str, Path]]):
-        """Construct a Variants object from GVL files. The path(s) must end with `.gvl`.
-
-        Parameters
-        ----------
-        path : Union[str, Path, Dict[str, Path]]
-            Path to the GVL file(s).
-
-        Returns
-        -------
-        Variants
-        """
-        records = Records.from_gvl_arrow(path)
-        genotypes = ZarrGenos(path)
+        genotypes = VCFGenos(vcf, records.contig_offsets)
         return cls(records, genotypes)
 
-    # TODO: read sample names from .psam file by using #IID or IID column. Implement a .psam reader.
     @classmethod
-    def from_pgen(
-        cls, pgen: Union[str, Path, Dict[str, Path]], sample_names: ArrayLike
-    ):
+    def from_pgen(cls, pgen: Union[str, Path, Dict[str, Path]]):
         """Currently does not support multi-allelic sites, but does support *split*
         multi-allelic sites. Note that SVs and "other" variants are also not supported.
         A PGEN can be prepared from a VCF by running:
         ```bash
         bcftools view -i 'TYPE="snp" || TYPE="indel"' <file.bcf> \\
         | bcftools norm \\
             -a \\
@@ -159,26 +135,53 @@
         ```
         """
         if isinstance(pgen, str):
             pgen = Path(pgen)
 
         if isinstance(pgen, Path):
             pgen = {"_all": pgen}
+
+        psams: Dict[str, pl.DataFrame] = {}
+        samples = None
+        for contig, path in pgen.items():
+            with open(path.with_suffix(".psam")) as f:
+                cols = [c.strip("#") for c in f.readline().strip().split()]
+
+            psam = pl.read_csv(
+                path.with_suffix(".psam"),
+                separator="\t",
+                has_header=False,
+                skip_rows=1,
+                new_columns=cols,
+                dtypes={
+                    "FID": pl.Utf8,
+                    "IID": pl.Utf8,
+                    "SID": pl.Utf8,
+                    "PAT": pl.Utf8,
+                    "MAT": pl.Utf8,
+                    "SEX": pl.Utf8,
+                },
+            )
+
+            if samples is None:
+                samples = psam["IID"].to_numpy()
+            else:
+                intersection = np.intersect1d(samples, psam["IID"].to_numpy())
+                if np.any(samples != intersection):
+                    raise ValueError("Sample names do not match across contigs.")
+
+            psams[contig] = psam
+        assert samples is not None
+
         records = Records.from_pvar(
             {c: p.with_suffix(".pvar") for c, p in pgen.items()}
         )
-        sample_names = np.atleast_1d(np.asarray(sample_names))
-        genotypes = PgenGenos(pgen, sample_names)
-        return cls(records, genotypes)
 
-    def in_memory(self):
-        if not isinstance(self.genotypes, NumpyGenos):
-            genotypes = NumpyGenos.from_recs_genos(self.records, self.genotypes)
-            return self.__class__(self.records, genotypes)
-        return self
+        genotypes = PgenGenos(pgen, samples, records.contigs)
+        return cls(records, genotypes)
 
     def subset_samples(self, samples: ArrayLike):
         samples = np.atleast_1d(np.asarray(samples, dtype=str))
         geno_sample_idxs, sample_idxs = np.intersect1d(
             self.genotypes.samples, samples, return_indices=True
         )[1:]
         if len(sample_idxs) != len(samples):
@@ -275,99 +278,13 @@
         )
 
         return (
             DenseGenotypes(
                 recs.positions,
                 recs.size_diffs,
                 recs.refs,
-                recs.alts,
-                genos,
-                recs.offsets,
-            ),
-            max_ends,
-        )
-
-    def vidx(
-        self,
-        contigs: ArrayLike,
-        starts: ArrayLike,
-        length: int,
-        samples: ArrayLike,
-        ploidies: ArrayLike,
-    ):
-        if not isinstance(self.genotypes, VIdxGenos):
-            raise ValueError(
-                f"Genotypes {self.genotypes} does not support vectorized indexing."
-            )
-
-        contigs = np.atleast_1d(np.asarray(contigs, dtype=str))
-        starts = np.atleast_1d(np.asarray(starts, dtype=int))
-        samples = np.atleast_1d(np.asarray(samples, dtype=str))
-        ploidies = np.atleast_1d(np.asarray(ploidies, dtype=int))
-
-        recs = self.records.vidx_vars_in_range(contigs, starts, length)
-        if recs is None:
-            return None
-
-        genos = self.genotypes.vidx(
-            contigs, recs.start_idxs, recs.end_idxs, samples, ploidies
-        )
-
-        return DenseGenotypes(
-            recs.positions,
-            recs.size_diffs,
-            recs.refs,
-            recs.alts,
-            genos,
-            recs.offsets,
-        )
-
-    def vidx_for_haplotype_construction(
-        self,
-        contigs: ArrayLike,
-        starts: ArrayLike,
-        length: int,
-        samples: ArrayLike,
-        ploidies: ArrayLike,
-    ):
-        if not isinstance(self.genotypes, VIdxGenos):
-            raise ValueError(
-                f"Genotypes {self.genotypes} does not support vectorized indexing."
-            )
-
-        contigs = np.atleast_1d(np.asarray(contigs, dtype=np.str_))
-        starts = np.atleast_1d(np.asarray(starts, dtype=np.int32))
-        samples = np.atleast_1d(np.asarray(samples, dtype=np.str_))
-        ploidies = np.atleast_1d(np.asarray(ploidies, dtype=np.intp))
-
-        recs, max_ends = self.records.vidx_vars_in_range_for_haplotype_construction(
-            contigs, starts, length
-        )
-        if recs is None:
-            return None, max_ends
-
-        unique_samples, inverse = np.unique(samples, return_inverse=True)
-        if missing := set(unique_samples).difference(self.samples):
-            raise ValueError(f"Samples {missing} were not found")
-        key_idx, query_idx = np.intersect1d(
-            self.samples, unique_samples, return_indices=True, assume_unique=True
-        )[1:]
-        sample_idx = key_idx[query_idx[inverse]]
-
-        if (ploidies >= self.ploidy).any():
-            raise ValueError("Ploidies requested exceed maximum ploidy")
-
-        genos = self.genotypes.vidx(
-            contigs, recs.start_idxs, recs.end_idxs, sample_idx, ploidies
-        )
-
-        return (
-            DenseGenotypes(
-                recs.positions,
-                recs.size_diffs,
-                recs.refs,
                 recs.alts,
                 genos,
                 recs.offsets,
             ),
             max_ends,
         )
```

### Comparing `genvarloader-0.3.1/python/genvarloader/variants/records.py` & `genvarloader-0.3.2/python/genvarloader/variants/records.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from pathlib import Path
 from textwrap import dedent
-from typing import Dict, Iterable, List, Literal, Optional, Tuple, Union, overload
+from typing import Dict, Iterable, List, Literal, Optional, Tuple, Union, cast, overload
 
 import numba as nb
 import numpy as np
 import polars as pl
+import pyarrow as pa
 from attrs import define
 from loguru import logger
 from numpy.typing import ArrayLike, NDArray
 from tqdm.auto import tqdm
 from typing_extensions import Self, assert_never
 
 from ..utils import lengths_to_offsets, normalize_contig_name, offsets_to_lengths
@@ -26,28 +27,28 @@
 class VLenAlleles:
     """Variable length alleles.
 
     Create VLenAlleles from a polars Series of strings:
     >>> alleles = VLenAlleles.from_polars(pl.Series(["A", "AC", "G"]))
 
     Create VLenAlleles from offsets and alleles:
-    >>> offsets = np.array([0, 1, 3, 4], np.uint32)
+    >>> offsets = np.array([0, 1, 3, 4], np.uint64)
     >>> alleles = np.frombuffer(b"AACG", "|S1")
     >>> alleles = VLenAlleles(offsets, alleles)
 
     Get a single allele:
     >>> alleles[0]
     b'A'
 
     Get a slice of alleles:
     >>> alleles[1:]
     VLenAlleles(offsets=array([0, 2, 3]), alleles=array([b'AC', b'G'], dtype='|S1'))
     """
 
-    offsets: NDArray[np.uint32]
+    offsets: NDArray[np.int64]
     alleles: NDArray[np.bytes_]
 
     @overload
     def __getitem__(self, idx: int) -> NDArray[np.bytes_]: ...
 
     @overload
     def __getitem__(self, idx: slice) -> "VLenAlleles": ...
@@ -72,15 +73,15 @@
         if start is None:
             start = 0
         elif start < 0:
             start += len(self)
 
         # handle empty result
         if start >= len(self) or (stop is not None and stop <= start):
-            return VLenAlleles(np.empty(0, np.uint32), np.empty(0, "|S1"))
+            return VLenAlleles(np.empty(0, np.uint64), np.empty(0, "|S1"))
 
         if stop is None:
             stop = len(self)
         elif stop < 0:
             stop += len(self)
         stop += 1
         new_offsets = self.offsets[start:stop].copy()
@@ -95,31 +96,42 @@
 
     @property
     def nbytes(self):
         return self.offsets.nbytes + self.alleles.nbytes
 
     @classmethod
     def from_polars(cls, alleles: pl.Series):
-        offsets = np.r_[np.uint32(0), alleles.str.len_bytes().cum_sum().to_numpy()]
+        offsets = np.empty(len(alleles) + 1, np.int64)
+        offsets[0] = 0
+        offsets[1:] = alleles.str.len_bytes().cast(pl.Int64).cum_sum().to_numpy()
         flat_alleles = np.frombuffer(
             alleles.str.concat("").to_numpy()[0].encode(), "S1"
         )
         return cls(offsets, flat_alleles)
 
+    def to_polars(self):
+        n_alleles = len(self)
+        offset_buffer = pa.py_buffer(self.offsets)
+        allele_buffer = pa.py_buffer(self.alleles)
+        string_arr = pa.LargeStringArray.from_buffers(
+            n_alleles, offset_buffer, allele_buffer
+        )
+        return pl.Series(string_arr)
+
     @staticmethod
     def concat(*vlen_alleles: "VLenAlleles"):
         if len(vlen_alleles) == 0:
-            return VLenAlleles(np.array([0], np.uint32), np.array([], "|S1"))
+            return VLenAlleles(np.array([0], np.int64), np.array([], "|S1"))
         elif len(vlen_alleles) == 1:
             return vlen_alleles[0]
 
         nuc_per_allele = np.concatenate(
             [offsets_to_lengths(v.offsets) for v in vlen_alleles]
         )
-        offsets = lengths_to_offsets(nuc_per_allele, np.uint32)
+        offsets = lengths_to_offsets(nuc_per_allele, np.int64)
         alleles = np.concatenate([v.alleles for v in vlen_alleles])
         return VLenAlleles(offsets, alleles)
 
 
 @define
 class RecordInfo:
     """Information about sets of records corresponding to range queries.
@@ -140,46 +152,46 @@
         Alternate alleles.
     start_idxs : NDArray[np.int32]
         Shape: (n_queries)
         Start indices of the records for each query.
     end_idxs : NDArray[np.int32]
         Shape: (n_queries)
         End indices of the records for each query.
-    offsets : NDArray[np.uint32]
+    offsets : NDArray[np.int32]
         Shape: (n_queries + 1).
         Offsets for the records such that records[offsets[i]:offsets[i+1]] are the records
         for the i-th query.
     """
 
     positions: NDArray[np.int32]  # (n_variants)
     size_diffs: NDArray[np.int32]  # (n_variants)
     refs: VLenAlleles
     alts: VLenAlleles
     start_idxs: NDArray[np.int32]  # (n_queries)
     end_idxs: NDArray[np.int32]  # (n_queries)
-    offsets: NDArray[np.uint32]  # (n_queries + 1)
+    offsets: NDArray[np.int32]  # (n_queries + 1)
 
     @property
     def n_queries(self):
         return len(self.start_idxs)
 
     @classmethod
     def empty(cls, n_queries: int):
         return cls(
             positions=np.empty(n_queries, np.int32),
             size_diffs=np.empty(n_queries, np.int32),
             refs=VLenAlleles(
-                np.zeros(n_queries + 1, np.uint32), np.empty(n_queries, "S1")
+                np.zeros(n_queries + 1, np.uint64), np.empty(n_queries, "S1")
             ),
             alts=VLenAlleles(
-                np.zeros(n_queries + 1, np.uint32), np.empty(n_queries, "S1")
+                np.zeros(n_queries + 1, np.uint64), np.empty(n_queries, "S1")
             ),
             start_idxs=np.empty(n_queries, np.int32),
             end_idxs=np.empty(n_queries, np.int32),
-            offsets=np.zeros(n_queries + 1, np.uint32),
+            offsets=np.zeros(n_queries + 1, np.int32),
         )
 
     @staticmethod
     def concat(
         *record_infos: "RecordInfo", how: Literal["separate", "merge"] = "separate"
     ):
         if len(record_infos) == 0:
@@ -193,17 +205,17 @@
         alts = VLenAlleles.concat(*(r.alts for r in record_infos))
         start_idxs = np.concatenate([r.start_idxs for r in record_infos])
         end_idxs = np.concatenate([r.end_idxs for r in record_infos])
         v_per_query = np.concatenate(
             [offsets_to_lengths(r.offsets) for r in record_infos]
         )
         if how == "separate":
-            offsets = lengths_to_offsets(v_per_query, np.uint32)
+            offsets = lengths_to_offsets(v_per_query)
         elif how == "merge":
-            offsets = np.array([0, v_per_query.sum()], np.uint32)
+            offsets = np.array([0, v_per_query.sum()], np.int32)
         else:
             assert_never(how)
         return RecordInfo(
             positions=positions,
             size_diffs=size_diffs,
             refs=refs,
             alts=alts,
@@ -259,15 +271,17 @@
         }
 
         if cls.gvl_arrow_exists(vcf, arrow_paths):
             return cls.from_gvl_arrow(arrow_paths)
 
         if multi_contig_source:
             start_df = cls.read_vcf(vcf["_all"])
-            start_dfs = start_df.partition_by("#CHROM", as_dict=True)
+            start_dfs = start_df.partition_by(
+                "#CHROM", as_dict=True, maintain_order=True
+            )
             del start_df
         else:
             start_dfs: Dict[str, pl.DataFrame] = {}
             for contig, path in vcf.items():
                 start_dfs[contig] = cls.read_vcf(path)
 
         start_dfs, end_dfs = cls.process_start_df(start_dfs)
@@ -295,46 +309,47 @@
     def read_vcf(vcf_path: Path):
         if not CYVCF2_INSTALLED:
             raise ImportError(
                 "cyvcf2 is not installed. Please install it with `pip install cyvcf2`"
             )
 
         vcf = cyvcf2.VCF(str(vcf_path))  # pyright: ignore
-        n_variants = vcf.num_records
-        chroms = [None] * n_variants
+        n_variants = cast(int, vcf.num_records)
+        chroms: List[Optional[str]] = [None] * n_variants
         positions = np.empty(n_variants, dtype=np.int32)
-        refs = [None] * n_variants
-        alts = [None] * n_variants
-        non_snp_non_indel = False
+        refs: List[Optional[str]] = [None] * n_variants
+        alts: List[Optional[str]] = [None] * n_variants
+        sv_or_unknown = False
         with tqdm(
             total=n_variants, desc=f"Scanning variants from {vcf_path.name}"
         ) as pbar:
             for i, v in enumerate(vcf):
-                if not v.is_snp and not v.is_indel:
-                    non_snp_non_indel = True
-                    continue
-                chroms[i] = v.CHROM
-                positions[i] = v.POS
-                refs[i] = v.REF
-                alt = v.ALT
-                # TODO: punt multi-allelics. also punt missing ALT (aka the * allele)?
+                chroms[i] = cast(str, v.CHROM)
+                positions[i] = cast(int, v.POS)  # 1-indexed
+                if v.is_sv or v.var_type == "unknown":
+                    if not sv_or_unknown:
+                        logger.warning(
+                            f"VCF file {vcf_path} contains structural or unknown variants. These variants will be ignored."
+                        )
+                        sv_or_unknown = True
+                    # use placeholder that makes ilen = 0 so it doesn't affect anything downstream
+                    alt = "N" * len(v.REF)
+                else:
+                    alt = cast(List[str], v.ALT)
+                refs[i] = cast(str, v.REF)
+                # TODO: multi-allelics. Also, missing ALT (aka the * allele)?
                 if len(alt) != 1:
                     raise RuntimeError(
                         f"""VCF file {vcf_path} contains multi-allelic or overlappings
                         variants which are not yet supported by GenVarLoader. Normalize 
                         the VCF with `bcftools norm -f <reference.fa>
                         -a --atom-overlaps . -m - <file.vcf>`"""
                     )
                 alts[i] = alt[0]
                 pbar.update()
-        if non_snp_non_indel:
-            logger.warning(
-                f"""VCF file {vcf_path} contains non-SNP and non-INDEL variants. 
-                These variants will be ignored."""
-            )
         return pl.DataFrame(
             {
                 "#CHROM": chroms,
                 "POS": positions,
                 "REF": refs,
                 "ALT": alts,
             }
@@ -353,15 +368,17 @@
         arrow_paths = {c: p.with_suffix(".gvl.arrow") for c, p in pvar.items()}
 
         if cls.gvl_arrow_exists(pvar, arrow_paths):
             return cls.from_gvl_arrow(arrow_paths)
 
         if multi_contig_source:
             start_df = cls.read_pvar(pvar["_all"])
-            start_dfs = start_df.partition_by("#CHROM", as_dict=True)
+            start_dfs = start_df.partition_by(
+                "#CHROM", as_dict=True, maintain_order=True
+            )
         else:
             start_dfs: Dict[str, pl.DataFrame] = {}
             for contig, path in pvar.items():
                 start_dfs[contig] = cls.read_pvar(path)
 
         start_dfs, end_dfs = cls.process_start_df(start_dfs)
 
@@ -405,15 +422,15 @@
         return pvar
 
     @staticmethod
     def gvl_arrow_exists(
         sources: Union[Path, Dict[str, Path]], arrow: Union[Path, Dict[str, Path]]
     ) -> bool:
         # TODO: check if files were created after the last breaking change to the gvl.arrow format
-        # check if the files exist
+        # check if the files exist and are more recent than the sources
         if isinstance(arrow, Path):
             assert isinstance(sources, Path)
             if not arrow.exists():
                 return False
             if not arrow.stat().st_mtime >= sources.stat().st_mtime:
                 return False
         else:
@@ -496,15 +513,15 @@
                     END=pl.col("POS")
                     - pl.col("ILEN").clip(upper_bound=0),  #! end-inclusive
                 )
                 .with_row_count("VAR_IDX")
                 .select(
                     pl.all().sort_by("END"),
                     # make E2S_IDX relative to each contig
-                    pl.int_range(0, pl.count(), dtype=pl.UInt32)
+                    pl.int_range(0, pl.count(), dtype=pl.Int32)
                     .sort_by("END")
                     .reverse()
                     .rolling_min(df.height, min_periods=1)
                     .reverse()
                     .alias("E2S_IDX"),
                 )
                 .select("#CHROM", "END", "ILEN", "VAR_IDX", "E2S_IDX")
@@ -515,15 +532,15 @@
             _starts = ends["POS"].to_numpy()
             _ends = ends["END"].to_numpy()
             was_ends = np.empty(len(_ends) + 1, dtype=_ends.dtype)
             was_ends[0] = 0
             #! convert to end-exclusive, + 1
             was_ends[1:] = _ends + 1
             md_q = np.searchsorted(was_ends, _starts, side="right") - 1
-            ends = ends.with_columns(MD_Q=md_q).select(
+            ends = ends.with_columns(MD_Q=md_q).select(  # type: ignore
                 "#CHROM", "END", "MD_Q", "ILEN", "E2S_IDX"
             )
 
             end_dfs[contig] = ends
 
         return start_dfs, end_dfs
 
@@ -553,15 +570,15 @@
             e_df = end_dfs[contig]
             contig_offsets[contig] = contig_offset
             contig_offset += s_df.height
             v_starts[contig] = s_df["POS"].to_numpy()
             v_diffs[contig] = s_df["ILEN"].to_numpy()
             v_ends[contig] = e_df["END"].to_numpy()
             v_diffs_sorted_by_ends[contig] = e_df["ILEN"].to_numpy()
-            e2s_idx[contig] = np.empty(e_df.height + 1, dtype=np.uint32)
+            e2s_idx[contig] = np.empty(e_df.height + 1, dtype=np.int32)
             e2s_idx[contig][:-1] = e_df["E2S_IDX"].to_numpy()
             e2s_idx[contig][-1] = e_df.height
             max_del_q[contig] = e_df["MD_Q"].to_numpy()
 
             # no multi-allelics
             ref[contig] = VLenAlleles.from_polars(s_df["REF"])
             alt[contig] = VLenAlleles.from_polars(s_df["ALT"])
@@ -581,39 +598,34 @@
 
     def vars_in_range(
         self,
         contig: str,
         starts: ArrayLike,
         ends: ArrayLike,
     ) -> RecordInfo:
-        starts = np.atleast_1d(np.asarray(starts, dtype=int))
-        ends = np.atleast_1d(np.asarray(ends, dtype=int))
+        starts = np.atleast_1d(np.asarray(starts, dtype=np.int32))
+        ends = np.atleast_1d(np.asarray(ends, dtype=np.int32))
         n_queries = len(starts)
 
         _contig = normalize_contig_name(contig, self.contigs)
         if _contig is None:
             return RecordInfo.empty(n_queries)
 
-        _s_idxs = np.searchsorted(self.v_ends[_contig], starts)
-        # make idxs absolute
-        s_idxs = self.e2s_idx[_contig][_s_idxs] + self.contig_offsets[_contig]
-        e_idxs = (
-            np.searchsorted(self.v_starts[_contig], ends) + self.contig_offsets[_contig]
-        )
+        rel_s_idxs = self.find_relative_start_idx(_contig, starts)
+        rel_e_idxs = self.find_relative_end_idx(_contig, ends)
 
-        if s_idxs.min() == e_idxs.max():
+        if rel_s_idxs.min() == rel_e_idxs.max():
             return RecordInfo.empty(n_queries)
 
-        n_var_per_region = e_idxs - s_idxs
-        offsets = np.empty(len(n_var_per_region) + 1, dtype=np.uint32)
-        offsets[0] = 0
-        offsets[1:] = np.cumsum(n_var_per_region)
+        n_var_per_region = rel_e_idxs - rel_s_idxs
+        offsets = lengths_to_offsets(n_var_per_region)
 
-        rel_s_idxs = s_idxs - self.contig_offsets[_contig]
-        rel_e_idxs = e_idxs - self.contig_offsets[_contig]
+        # make idxs absolute
+        s_idxs = rel_s_idxs + self.contig_offsets[_contig]
+        e_idxs = rel_e_idxs + self.contig_offsets[_contig]
 
         positions = np.concatenate(
             [self.v_starts[_contig][s:e] for s, e in zip(rel_s_idxs, rel_e_idxs)]
         )
         size_diffs = np.concatenate(
             [self.v_diffs[_contig][s:e] for s, e in zip(rel_s_idxs, rel_e_idxs)]
         )
@@ -630,14 +642,27 @@
             refs=ref,
             alts=alt,
             start_idxs=s_idxs,
             end_idxs=e_idxs,
             offsets=offsets,
         )
 
+    def find_relative_start_idx(
+        self, contig: str, starts: NDArray[np.int32]
+    ) -> NDArray[np.int32]:
+        s_idx_by_end = np.searchsorted(self.v_ends[contig], starts)
+        rel_s_idx = self.e2s_idx[contig][s_idx_by_end]
+        return rel_s_idx
+
+    def find_relative_end_idx(
+        self, contig: str, ends: NDArray[np.int32]
+    ) -> NDArray[np.int32]:
+        rel_e_idx = np.searchsorted(self.v_starts[contig], ends)
+        return rel_e_idx
+
     def vars_in_range_for_haplotype_construction(
         self,
         contig: str,
         starts: ArrayLike,
         ends: ArrayLike,
     ) -> Tuple[RecordInfo, NDArray[np.int32]]:
         starts = np.atleast_1d(np.asarray(starts, dtype=np.int32))
@@ -664,18 +689,15 @@
         # make idxs absolute
         s_idxs += self.contig_offsets[_contig]
         e_idxs += self.contig_offsets[_contig]
 
         if s_idxs.min() == e_idxs.max():
             return RecordInfo.empty(n_queries), ends
 
-        np.concatenate(
-            [np.arange(s, e, dtype=np.uint32) for s, e in zip(s_idxs, e_idxs)]
-        )
-        offsets = np.empty(n_queries + 1, dtype=np.uint32)
+        offsets = np.empty(n_queries + 1, dtype=np.int32)
         offsets[0] = 0
         np.cumsum(e_idxs - s_idxs, out=offsets[1:])
 
         rel_s_idxs = s_idxs - self.contig_offsets[_contig]
         rel_e_idxs = e_idxs - self.contig_offsets[_contig]
 
         positions = np.concatenate(
```

### Comparing `genvarloader-0.3.1/python/genvarloader/zarr.py` & `genvarloader-0.3.2/python/genvarloader/zarr.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/src/bigwig.rs` & `genvarloader-0.3.2/src/bigwig.rs`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/src/lib.rs` & `genvarloader-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/pgen/sample.ends.gvl.arrow` & `genvarloader-0.3.2/tests/data/pgen/sample.ends.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/pgen/sample.gvl.arrow` & `genvarloader-0.3.2/tests/data/pgen/sample.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/pgen/sample.pvar` & `genvarloader-0.3.2/tests/data/pgen/sample.pvar`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/filtered_sample.ends.gvl.arrow` & `genvarloader-0.3.2/tests/data/vcf/filtered_sample.ends.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.arrow` & `genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.arrow`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0` & `genvarloader-0.3.2/tests/data/vcf/filtered_sample.gvl.genos.zarr/0.0.0`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf` & `genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/filtered_sample.vcf.gz` & `genvarloader-0.3.2/tests/data/vcf/filtered_sample.vcf.gz`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/generate_ground_truth.py` & `genvarloader-0.3.2/tests/data/vcf/generate_ground_truth.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/data/vcf/sample.vcf` & `genvarloader-0.3.2/tests/data/vcf/sample.vcf`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/dataset/genotypes/test_dense2sparse.py` & `genvarloader-0.3.2/tests/dataset/genotypes/test_dense2sparse.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_fasta.py` & `genvarloader-0.3.2/tests/test_fasta.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_fasta_variants.py` & `genvarloader-0.3.2/tests/test_fasta_variants.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_loader.py` & `genvarloader-0.3.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_max_ends.py` & `genvarloader-0.3.2/tests/test_max_ends.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_pgen.py` & `genvarloader-0.3.2/tests/test_pgen.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/test_variants.py` & `genvarloader-0.3.2/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/tracks/bench_cpu_gpu.py` & `genvarloader-0.3.2/tests/tracks/bench_cpu_gpu.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/tracks/test_i2t_t2i.py` & `genvarloader-0.3.2/tests/tracks/test_i2t_t2i.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/tracks/test_random_nonoverlapping.py` & `genvarloader-0.3.2/tests/tracks/test_random_nonoverlapping.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/tests/tracks/utils.py` & `genvarloader-0.3.2/tests/tracks/utils.py`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/Cargo.lock` & `genvarloader-0.3.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `genvarloader-0.3.1/pyproject.toml` & `genvarloader-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genvarloader"
-version = "0.3.1"
+version = "0.3.2"
 description = "Pipeline for efficient genomic data processing."
 authors = [
     { name = "David Laub", email = "dlaub@ucsd.edu" },
     { name = "Aaron Ho", email = "aho@salk.edu" },
 ]
 readme = "README.md"
 repository = "https://github.com/mcvickerlab/genome-loader"
@@ -32,34 +32,31 @@
     "pybigwig>=0.3.22",
     "einops>=0.7.0",
     "typer>=0.11.0",
     "tbb>=2021.12.0",
 ]
 
 [project.scripts]
-genvarloader = 'cli:app'
+genvarloader = 'genvarloader.__main__:app'
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.4.2",
     "mypy>=1.6.0",
     "memray>=1.10.0",
     "py-spy>=0.3.14",
     "icecream>=2.1.3",
     "pytest-cases>=3.8.0",
     "pytest-cov>=4.1.0",
     "ruff>=0.0.292",
     "pre-commit>=3.5.0",
     "pytest-benchmark>=4.0.0",
+    "filelock>=3.13.1"
 ]
 
-[tool.poetry-dynamic-versioning]
-enable = true
-vcs = "git"
-
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin", "pandera.mypy"]
 
 [tool.ruff]
 lint.ignore = ["E501"]
 
 [tool.pyright]
```

### Comparing `genvarloader-0.3.1/PKG-INFO` & `genvarloader-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: genvarloader
-Version: 0.3.1
+Version: 0.3.2
 Requires-Dist: pytest >=7.4.2 ; extra == 'dev'
 Requires-Dist: mypy >=1.6.0 ; extra == 'dev'
 Requires-Dist: memray >=1.10.0 ; extra == 'dev'
 Requires-Dist: py-spy >=0.3.14 ; extra == 'dev'
 Requires-Dist: icecream >=2.1.3 ; extra == 'dev'
 Requires-Dist: pytest-cases >=3.8.0 ; extra == 'dev'
 Requires-Dist: pytest-cov >=4.1.0 ; extra == 'dev'
 Requires-Dist: ruff >=0.0.292 ; extra == 'dev'
 Requires-Dist: pre-commit >=3.5.0 ; extra == 'dev'
 Requires-Dist: pytest-benchmark >=4.0.0 ; extra == 'dev'
+Requires-Dist: filelock >=3.13.1 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE.txt
 Summary: Pipeline for efficient genomic data processing.
 Author-email: David Laub <dlaub@ucsd.edu>, Aaron Ho <aho@salk.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

