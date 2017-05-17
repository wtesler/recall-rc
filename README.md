# recall-rc
A shell script for persistently storing and recalling previously entered commands.

add to your `.zshrc`, `.bash_profile`, or `.bashrc` with one line: `source ~/.recall-rc`

It has the following commands:

      `help` - Show help information
      `save` - Save the previously entered command. i.e. `recall save`
      `list` - Show all saved entries. i.e. `recall list`
      `remove` INDEX - Remove an entry by index. i.e. `recall remove 63`
      `INDEX `- reuse the entry at the given index. i.e. `recall 79`
