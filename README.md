# atgcN_count

## 1 Introduction

`atgcN_count` is a tool to stat the counts and percentage of each base in fasta file.

## 2 Installation

    pip install atgcN_count

There will be a command `atgcN_count` created under the same directory as your `pip` command.

## 3 Usage

    $ atgcN_count

    usage: atgcN_count[-h] [-i <file>] [-v] [-d <int>] [-N]

    To stat the counts of each base in a fasta file. By Guanliang MENG.

    optional arguments:
      -h, --help  show this help message and exit
      -i <file>   input fasta file
      -v          also output statistics for each sequence [False]
      -d <int>    decimals for output result [2]
      -N          do not take non-ATGC bases into account when caculate percentage
                  [False]


### example

    $ atgcN_count -i SRR836315_COX1_sample.fa -v
    >scaffold358;COX1;[1567:3117](+)
    A 417 26.9
    T 487 31.42
    G 282 18.19
    C 364 23.48
    A+T: 58.32
    G+C: 41.68
    non-ATGC: 0.0
    total bases: 1,550
    >NC_010642.1;COX1;[6279:7824](+)
    A 402 26.02
    T 479 31.0
    G 295 19.09
    C 369 23.88
    A+T: 57.02
    G+C: 42.98
    non-ATGC: 0.0
    total bases: 1,545

    statistics of all sequences:
    A 819 26.46
    T 966 31.21
    G 577 18.64
    C 733 23.68
    A+T: 57.67
    G+C: 42.33
    non-ATGC: 0.0
    total bases: 3,095

## Author
Guanliang MENG

## Citation
Currently I have no plan to publish `atgcN_count`.





