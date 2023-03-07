
In the previous chapters, you learnt how to move around in the Unix filesystem and access files. 
This chapter will show you how to explore the data in those files. 
The commands we’ll use are fairly simple, but are solid building blocks of more sophisticated traitement pipelines.

First, go to the `data` directory with the `cd` command:

```bash
cd data
```

Check you are in the expected directory with `pwd`:

```bash
pwd
```

The result should be `/root/data`. This directory should contain 3 files you could find with the command `ls`.

## Displaying file contents

### *cat*

A first command to display file contents is `cat`:

```bash
cat gnagnagna.fasta
```

This command will print the content of the file *gnagnagna.fasta* in your terminal.


Now, print the content of the file *belebele.fasta*.

**Question:** What are the last three nucleotides of the file *belebele.fasta*?
- ELE
- ATT
- ATC
- BEL

<details>
<summary>Answer</summary>

ATT

</details>
