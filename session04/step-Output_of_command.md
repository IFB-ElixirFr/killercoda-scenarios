## Output of a Unix command

By default, as you have seen so far, the result of a Unix command is printed on the screen.

For example, to extract the genomic location for the gene *gene-SAOUHSC_00079* from the file `belebele.bed` with the `grep` command:

1. Go in the `data` directory.
2. Check the file `belebele.bed` is present.
3. Extract the location of the gene *gene-SAOUHSC_00079*.

```bash
cd data
ls
grep gene-SAOUHSC_00079 belebele.bed
```

The outputs of the commands `ls` and `grep` are printed on the terminal.

The standard output of a command is called **stdout**.

This schema illustrates the output stream of a command:

![output printed on the screen](./assets/stream_out.png)

By default, **stdout** is set to the screen.

But you can change this behavior and redirect **stdout** to a file.

You can use the `1>` operator to do this or more simply, `>`:

```bash
grep gene-SAOUHSC_00079 belebele.bed > gene.bed
```

With previsous command, nothing has been printed on the screen, but a new file `gene.bed` has been created

```bash
ls
```

You can show its content using the `cat` command:
```bash
cat gene.bed
```
Its content is just the same as the result of the grep command.

The `>` symbol is one of the **redirection** operators.

The next figure illustrates the **stdout** redirection to a file:

![output printed into a file](./assets/stream_outfile.png)

⚠️ if the file already exists, it’s content will be replaced by the output of your command

If you run the same `grep` as before but searching for a different gene, the output file will be overwritten

```bash
grep gene-SAOUHSC_00078 belebele.bed > gene.bed
cat gene.bed
```

To avoid this, you may use the `>>` operator which appends the output of your command to the end of an existing file.

```bash
grep gene-SAOUHSC_00079 belebele.bed > gene.bed
grep gene-SAOUHSC_00078 belebele.bed >> gene.bed
cat gene.bed
```

**Question:** Which command appends its result at the end of the file `toto`?

- `grep foo file1 > toto`
- `grep foo file1 >> toto`
- `grep foo toto > file1`

<details>
<summary>Answer</summary>

`grep foo file1 >> toto`

</details>
