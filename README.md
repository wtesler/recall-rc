# recall-rc
A shell script for persistently storing and recalling previously entered commands.

add to your `.zshrc`, `.bash_profile`, or `.bashrc` with one line: `source ~/.recall-rc`

Use it by entering `recall X` into your command line, where `X` is one of the following commands:

      `save` - Save the previously entered command. i.e. `recall save`
      `list` - Show all saved entries. i.e. `recall list`
      `remove` INDEX - Remove an entry by index. i.e. `recall remove 63`
      `INDEX `- reuse the entry at the given index. i.e. `recall 79`
      `help` - Show help information
