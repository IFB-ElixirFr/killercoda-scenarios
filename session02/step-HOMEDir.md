When used without any argument, the `cd` command will set the current working directory to your HOME directory. 
This HOME directory is the place where a user can store his or her files. 

Move yourself to your HOME directory using the `cd` command and print the current working directory using the `pwd` command:

```bash
cd 
pwd
```

The symbol for the HOME directory is `~` (tilde). This character can be accessed with a PC keyboard using <kbd>AltGr</kbd> + <kbd>2</kbd>. With a Mac OSX keyboard, it may be accessed using <kbd>option</kbd> + <kbd>n</kbd>. 

In the example below, we successively go to the `/tmp` directory and then to the `/root/test` directory:

```bash
cd /tmp
pwd
cd ~/test
pwd
```

However, note that the HOME directory is not always the right place to store large files, particularly on a cluster with shared resources. Ask your administrator about appropriate guidelines!


To answer the next question, type the following commands:

```bash
cd /shared/bank/nr
cd ~/test
cd
```

**Question:** What is the current working directory?

- `/shared/bank/nr`
- `test`
- your HOME directory
- `nr`
- `/root`
- `/root/test`

<details>

`/root` that is also *your HOME directory*

</details>
