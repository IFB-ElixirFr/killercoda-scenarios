### *wc*

`wc` is the **w**ord **c**ount command. 
It counts the number of lines, words, and characters in files:

```bash
wc gnagnagna.bed
``` 

The file `gnagnagna.bed` has, from left to right: 8 lines, 48 words and 364 characters.

To output only the number of lines, run `wc` with the option *-l*:

```bash
wc -l gnagnagna.bed
``` 

**Question:** How many lines has the file `gnagnagna.fasta`?
- 5
- 6
- 28
- 67

<details>
<summary>Answer</summary>

```bash
$ wc -l gnagnagna.fasta 
6 gnagnagna.fasta
```

6 lines

</details>

