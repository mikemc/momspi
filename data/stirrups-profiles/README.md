
fettweis2019thev used STIRRUPS (fettweis2012spec) for species-level assignment of vaginal samples, and deposited the profiles in the HMP DAC.
The STIRRUPS profiles in the HMP DAC can be found by the query

```
sample.study_name in ["MOMS-PI"] and sample.body_site in ["vagina"] and file.node_type in ["abundance_matrix"] and file.matrix_type in ["16s_community"] and file.format in ["tbl"]
```

I downloaded the profiles using the portal client (https://github.com/IGS/portal_client), created a checksum list, and made them read-only with

```sh
portal_client --manifest hmp_manifest_4abcc24e0d.tsv
md5sum *.txt > stirrups-profiles.md5
chmod -w *
```
