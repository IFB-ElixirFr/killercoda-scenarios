The `tree` command displays the tree-like organization of files and sub-directories contained in a particular directory.

In the example below, the `tree` command displays the content of the `/shared` directory limited only to directories (option `-d`) and with only two levels of sub-directories (option `-L 2`):

```bash
tree -d -L 2 /shared
```

These directories were created to store genome files of different species.

From the previous command we deduce the  path from the root `/` to the `homo_sapiens` directory. This path is:

```bash
/shared/bank/homo_sapiens
```

As stated previously, because this path starts with an `/`, it is an absolute path. Starting from the root  `/`, we go through the `shared` directory, then `bank` directory to finally reach the target `homo_sapiens` directory.

Paths are used in many Unix commands, such as the `ls` (that stands for **l**i**s**t) command:

```bash
ls /shared/bank/homo_sapiens
```

This `ls` command lists the content of the specified directory (also named **argument** of the `ls` command).


**Question:** Using the `ls` command, which repositories are in the `/shared/bank/homo_sapiens` repository?

- `hg18`
- `hg19`
- `hg37`
- `hg38`

<details>
<summary>Answer</summary>

`hg19` and `hg38`

</details>

Remark: Usually `hg` stands for **h**uman **g**enome and the number denotes the sequence version.

**Question:** What is the absolute path of the parent directory of the folder `/shared/bank/bos_taurus`?

- `/`
- `/shared`
- `/shared/bank`

<details>
<summary>Answer</summary>

`/shared/bank`

</details>


**Question:** What is the absolute path of the folder `hg19/fasta` in `/shared/bank` ?

- `/shared/bank/homo_sapiens/hg19`
- `/shared/bank/homo_sapiens/hg19/fasta`
- `bank/homo_sapiens/hg19/fasta`

<details>
<summary>Answer</summary>

`/shared/bank/homo_sapiens/hg19/fasta`

</details>
