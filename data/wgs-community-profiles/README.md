
The WGS community profiles in the HMP DAC can be found by the query
```
sample.study_name in ["MOMS-PI"] and file.matrix_type in ["wgs_community"] and file.node_type in ["abundance_matrix"]
```

I downloaded the profiles using the portal client (https://github.com/IGS/portal_client), created a checksum list, and made them read-only with

```sh
portal_client --manifest hmp_manifest_fc10ece5f.tsv
md5sum *.txt > wgs-community-profiles.md5
chmod -w *
```
