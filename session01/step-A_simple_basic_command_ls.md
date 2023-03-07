The Bash shell provides you with a working space including files and directories.

A very useful command is `ls`, that **l**i**s**ts the content of a directory.
On your Unix terminal on the right, type `ls` and then press the <kbd>Enter</kbd> key.

The Bash shell should display `Data` that is a directory named `Data`.

Now, type the following command in your terminal (and press <kbd>Enter</kbd>) :

```bash
ls Data
```

The Bash shell should display 8 files in the `Data` directory.

Remarks : 
- Pay attention to the space character between `ls` and `Data`.
- Don't forget to press <kbd>Enter</kbd> to run commands.
- `ls` is the command **name**.
- `Data` is a directory name and an **argument** of the `ls` command.

### Options

Options modify the way a Unix command works.
In Bash, shell options start with a simple or double dash (`-` or `--`).

For example, with the `ls` command we can display the size of the files using the `--size` option. 

Lets try and type: 

```bash
ls --size Data
```

Now, the 8 files are displayed with their respective sizes (in blocks). 

You can use a short form for this option by replacing `--size` (long form) by `-s` (short form).

Usually, we use the `-h` option to display sizes in more **h**uman readable formats (*e.g.* 1K, 234M, 2G). 

You can use several options in the same command and you can even merge short form options using a single dash as prefix.

Example: type the following commands in your terminal. Both are equivalent.

```bash
ls --size -h Data
ls -sh Data
```

**Question:** Among the following commands, which ones are correct?
- `ls -s -h Data`
- `ls -sh Data`
- `ls -size -h Data`
- `ls --size -h Data`
- `ls --sizeh Data`
- `ls --size-h Data`
- `ls -h -s Data`
- `ls -hs Data`
- `ls -hsize Data`

<details>
<summary>Answer</summary>

- `ls -s -h Data`
- `ls -sh Data`
- `ls --size -h Data`
- `ls -h -s Data`
- `ls -hs Data`

</details>


### Summary

Here you've learnt that:
- You can execute a command by typing its name (optionally, with its options and arguments) and pressing <kbd>Enter</kbd>.
- You can add options to modify the command behavior.
- Options start with a dash `-` (short form) or a double dash `--` (long form).
- Several options of the short form can be combined (without space and after a single dash).
- Command name can be followed (or not) by an argument
