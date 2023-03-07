## Move (or rename) files and directories

The `mv` (**m**o**v**e) command takes 2 paths as arguments:

```bash
mv <source_path> <destination_path>
```

It moves the **source** to the **destination**.  
It works for files or directories.  
It is also used to rename files or directories.

Use the `mv` command to rename the file from `second_file.txt` to `file_2.txt` and to move it into your HOME directory:

```bash
cd
mv test/second_file.txt file_2.txt
tree
```

## Delete files and directories

The `rm` (**r**e**m**ove) command deletes files or directories.

Use `rm` to delete the file named `first_file.txt` from the directory `~/test`. Also use `tree` to check the organisation of files and directory from your HOME directory:

```bash
cd
rm test/first_file.txt
tree
```

To delete a directory, you need to use the `rm` command with the option `-r`:

```bash
rm -r <path_to_a_directory_to_delete>
```

Be very very careful with the `rm` command. There is no way to recover your deleted files in Unix!


**Question:** The `mv` command differs from the `rm` command by:

- `mv` applies to files or directories while `rm` applies to directories only
- `mv` requires 2 paths while `rm` requires only one path

<details>
<summary>Answer</summary>

`mv` requires 2 paths while `rm` requires only one path

</details>