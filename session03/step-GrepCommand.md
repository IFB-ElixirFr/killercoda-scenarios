## How to select part of a file

### *grep*

The `grep` command extracts lines matching a given pattern. 
A pattern can be a simple word or a more general expression, often termed **regular expression** (see [here](https://librarycarpentry.org/lc-data-intro/01-regular-expressions/) to learn more about these). 

For instance:

```bash
grep gene-SAOUHSC_00079 belebele.bed
```

**Question:** Print the line that contains the gene name *gene-SAOUHSC_00002*  in the file `belebele.bed`. What is the starting position (given in the 2nd column) of this gene?

- 750
- 2155
- 1561
- 3289

<details>
<summary>Answer</summary>

```bash
$ grep gene-SAOUHSC_00002 belebele.bed 
NC_007795.1     2155    3289    gene-SAOUHSC_00002      .       +
```

Starting position: 2155

</details>


Now, if you search for the gene *ABC* in the file `belebele.bed`:

```bash
grep ABC belebele.bed
```

You get no line containing the ABC gene name.

To count the number of lines containing the word *gene* word, add the `-c` option to the `grep` command:

```bash
grep -c gene belebele.bed
```

**Question:** Count the number of lines containing the word *cds* in `belebele.bed`
- 2270
- 2767
- 1878

<details>
<summary>Answer</summary>

```bash
$ grep -c cds belebele.bed 
2767
```

2767 cds

</details>

Here are other useful `grep` options:
- `-i`: searches the pattern in a case **i**nsensitive way.
- `-n`: adds the line **n**umber at the beginning of the output line.
- `-v`: prints the lines not containing the pattern (re**v**erse selection).

There are many other options: try `man grep`
