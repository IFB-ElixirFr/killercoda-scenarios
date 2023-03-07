When used without argument, the `cd` command will set the current working directory to your HOME directory. 
This HOME directory is the place where a user may store his or her files. 

```bash
cd 
pwd
```

The symbol for the HOME directory is `~` (tilde). This character can be accessed under a PC keyboard using <kbd>AltGr</kbd> + <kbd>2</kbd>. With a Mac OSX keyboard, it may be accessed using <kbd>option</kbd> + <kbd>n</kbd>. 

In the example below we successively go to the `/tmp` and then `/root/test` directories:

```bash
cd /tmp
pwd
cd ~/test
pwd
```

However, note that the HOME directory is not always the right place to store large files (particularly on a cluster with shared resources). 
Ask your administrator about appropriate guidelines!


To answer the next question, please type the 3 following commands:

```bash
cd /shared/bank/nr
cd ~/test
cd
```

What is the current working directory?

- [ ] `/shared/bank/nr`
- [ ] `test`
- [ ] your HOME directory
- [ ] `/shared/bank`
- [ ] `nr`
- [ ] `/root`
- [ ] `/root/test`

<details>
  <summary>Answer</summary>
  <p><tt>/root</tt> that is also <it>your HOME directory</it></p>
</details>
