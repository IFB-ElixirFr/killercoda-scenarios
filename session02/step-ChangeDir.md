The `cd` command (**c**hange **d**irectory) can be used to visit another directory in the file tree. 
The target directory must be specified using an absolute or a relative path. 

To experiment with the `cd` command, run the following commands:

```bash
cd /shared
cd bank/nr
cd ../homo_sapiens
```

**Question:** Could you guess the absolute path of your current working directory?

- `/shared/bank/`
- `/shared/homo_sapiens`
- `../bank/nr`
- `/shared/nr/homo_sapiens`
- `/shared/bank/homo_sapiens`

Verify your answer with `pwd`.

<details>
<summary>Answer</summary>

`/shared/bank/homo_sapiens`

</details>

### Automatic completion

To go from your current working directory to a target directory, you must specify the names of all intermediate directories. This can be time-consuming if the target directory is far away from your current directory. 
The key <kbd>Tab</kbd> triggers auto-completion. It means you just need to type the first letters of a directory, then press the <kbd>Tab</kbd> key, to get its full name completed. If there is more than one file or directory starting with the same letters, auto-completion will complete the name as far as it can. If you type a second time <kbd>Tab</kbd>, auto-completion will show you the available options.

The <kbd>Tab</kbd> key is perhaps the most used key in Unix!

Use the command `cd` and the <kbd>Tab</kbd> key to go into the `/shared/bank/bos_taurus/UMD3.1/star-2.7.2b/` directory.

**Question:** How many files are in the `/shared/bank/bos_taurus/UMD3.1/star-2.7.2b/` directory?

- 2
- 3
- 4
- 5

<details>
<summary>Answer</summary>

5

</details>
