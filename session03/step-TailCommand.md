### *tail*

If you just want to check the end of a file, you may use the `tail` command:

```bash
tail belebele.bed
```

The option *-n* is used the same way as with `head` to specify the number of lines shown (10 by default).


**Question:** Print the last line of the file `belebele.bed`. What is the name of the CDS in colmun 4?

- cds-YP_498677.1
- cds-YP_498678.1
- cds-YP_501500.1


<details>
<summary>Answer</summary>

```bash
$ tail -n 1 belebele.bed
NC_007795.1     2821010 2821148 cds-YP_501500.1 .       -
```

</details>

