## Input of a Unix command

The standard input of a command is named **stdin**

![input stream of a command](./assets/Stream_in_out.drawio.png)

By default, **stdin** is set to the keyboard. But you can change this behavior and read **stdin** from a file. You must use the `<` operator to do this.

The `tr` command translates (or deletes) characters from a text provided as input. If the file `seq1` contains one DNA sequence that we want to convert in RNA sequence (by replacing T by U) and change from upper case to lowercase, we could use the following command:

```bash
tr [AGCT] [agcu] < seq1 
```

Remark: `cat toto` is equivalent to `cat < toto` but `cat < toto` is seldom used.

![input stream of a command](./assets/Stream_infile_out.drawio.png)
