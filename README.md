# gene2bed

## merged into [skgGenomeTracks](https://github.com/skg-lab/skgGenomeTracks).

## installation

```
$ git clone https://github.com/yyoshiaki/gene2bed.git
```

Data files are included.

## usage

```
$ gene2bed.py -h                       
usage: gene2bed.py [-h] [-m MERGIN] species genelist output

Convert a gene list into a bed file.

positional arguments:
  species               human or mouse
  genelist              a gene list file
  output                output file

optional arguments:
  -h, --help            show this help message and exit
  -m MERGIN, --mergin MERGIN   mergin length
```

## example

```
$ ./gene2bed.py mouse example/genelist.txt example/out.bed
```

### input

genes.txt
```
Foxp3
Ctla4
Il2ra
```

### output

```
chr1    60887000        60915832        Ctla4   0       +
chr2    11642807        11693193        Il2ra   0       +
chrX    7573644 7595245 Foxp3   0       +
```

## references

- human : Gencode v30
- mouse : Gencode vM21

## data preparation

Only for the admins.

```
bash prep_data.sh
```
