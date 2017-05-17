# recall-rc
A shell script for persistently storing and re-invoking previously entered commands. Developers often copy commands that they want to remember into some file and then copy/paste them into the terminal. With `recall`, the commands can be stored persistently and re-invoked directly from the command line. Much easier than copy/pasting commands between files or attempting to navigate a long history. Even easier than using aliases.

Example:

```
> echo "Hello"
Hello
> recall save
> recall 0
Hello
> echo "Goodbye"
Goodbye
> recall save
> recall list
0. echo "Hello"
1. echo "Goodbye"
> recall 1
Goodbye
```

add to your `.zshrc`, `.bash_profile`, or `.bashrc` with one line: `source ~/.recall-rc`

Use it by entering `recall X` into your command line, where `X` is one of the following commands:

      `save` - Save the previously entered command. i.e. `recall save`
      `list` - Show all saved entries. i.e. `recall list`
      `remove` INDEX - Remove an entry by index. i.e. `recall remove 63`
      `INDEX `- reuse the entry at the given index. i.e. `recall 79`
      `help` - Show help information
