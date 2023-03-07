### *cut*

The `cut` command cuts out sections from each line of a file and writes the result to standard output.

It can be used to cut parts of a line by byte position, character and field (or column). 

Basically the `cut` command slices the lines to extract some text.
The main use of this command concerns the extraction of columns indicated by their number (first column is number 1).

Here is an example on how to extract the 3rd column of the file *belebele.bed*:

```bash
cut -f 3 belebele.bed
```

Multiple columns can be extracted using a comma between two column numbers or a '-' for a range of successive columns.

Try the extraction of the 3 first columns and the 5th column from the file *belebele.bed*:

```bash
cut -f 1-3,5 belebele.bed
```

You can change the delimiter between fields with the option *-d*. 

Look at the beginning of the file `peekaboo.csv` file (try the command `head peekaboo.csv`).
It contains 6 columns, separated by a comma.

**Question:** In the following commands, which one(s) extract the 2nd, 3rd, and 6th columns of the file `peekaboo.csv`?

- `cut -f 2,3,6 peekaboo.csv`
- `cut -f 2,3-6 peekaboo.csv`
- `cut -f 2,3,6 -d "," peekaboo.csv`
- `cut -f 2,3-6 -d "," peekaboo.csv`
- `cut -f 2-3,6 -d "," peekaboo.csv`
- `cut -f 2,3,6 -t "/t" peekaboo.csv`
- `cut -f 2-3,6 -t "/t" peekaboo.csv`


<details>
<summary>Answer</summary>

- `cut -f 2,3,6 -d "," peekaboo.csv`
- `cut -f 2-3,6 -d "," peekaboo.csv`

</details>



