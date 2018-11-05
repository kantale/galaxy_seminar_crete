# Useful files

## Galaxy server at IMBB (**temporary**)
* http://139.91.75.205 


## FastQ files:

```text
https://zenodo.org/record/583613/files/sample1-f.fq.gz
https://zenodo.org/record/583613/files/sample1-r.fq.gz
https://zenodo.org/record/583613/files/sample2-f.fq.gz
https://zenodo.org/record/583613/files/sample2-r.fq.gz
```


## Alignment results:

```text
https://www.dropbox.com/s/6219aba532fxtjw/file1.bam?dl=1
https://www.dropbox.com/s/f7zs4uu0j26znjg/file2.bam?dl=1
```

## BAM file

```
https://zenodo.org/record/60520/files/GIAB-Ashkenazim-Trio-hg19.gz?download=1
```

## Variant Calling result

```
https://www.dropbox.com/s/412m4z57ezr9oqd/freebayes_result.vcf?dl=1
```

## SnpEff annotation result

```
https://www.dropbox.com/s/0uh3s9rznv0lolb/SnpEff_html.zip?dl=1
https://www.dropbox.com/s/oowvo7n4gob470w/SnpEff_html.html?dl=1
https://www.dropbox.com/s/yi4zb0r2mx639hl/SnpEff_vcf.vcf?dl=1
```

## Trio information file

```text
https://zenodo.org/record/60520/files/GIAB-Ashkenazim-Trio.txt?download=1
```

## Gemini queries

### How maby "novel" variants that are not annotated in dbSNP database?


```
SELECT count(*) FROM variants WHERE in_dbsnp == 0
```

### How many variants within the POLRMT gene?


```
SELECT rs_ids, aaf_esp_ea, impact, clinvar_disease_name, clinvar_sig FROM variants WHERE filter is NULL and gene = 'POLRMT'
```

### At how many sites does child have a non-reference allele?

```
SELECT * from variants gt_types.HG002_NA24385_son <> HOM_REF 
```

