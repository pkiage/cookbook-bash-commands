# Table of Contents
[toc]

# Getting Help
## Check if a command is shell built-in or executable file 
This helps in getting help since MAN pages are available only for executable files.
### Generic: check type of command
```shell
type <command>
```

#### Example: MAN Page type
```shell
type man
```

#### Example: Help type
```shell
type help
```

## Help pages
Help pages are available for both built-in commands and executable files
### Generic: Help for command
For built-in commands (-dms only works in this case):
```shell
help <command>
```

For built-in commands and excecutable files:
```shell
<command> --help
```

#### Example: Help for help
```shell
help --help
```

#### Example: Help for help
```shell
help help
```

#### Example: Help for man
```shell
man --help
```

## MAN Pages
### Generic: MAN Page for command
```shell
man <command>
```

#### Example: MAN Page for man
```shell
man man
```
### Navigating an open MAN Page
#### Getting help on navigating an open MAN Pages
```shell
man <command>
```
Then once in manual entry press h on keyboad
#### Exit MAN Page
```shell
man <command>
```
To exit opened manual entry press q on keyboard

### Search manual page names and descriptions using man -k
#### Generic: Search for 'string' in manual page names and descriptions
```shell
man -k <string>
```

##### Example: Search for 'manual' in manual page names and descriptions
```shell
man -k manual
```

### Search manual page names and descriptions using apropos
#### Generic: Search for 'string' in manual page names and descriptions
```shell
apropos <string>
```

##### Example: Search for 'manual' in manual page names and descriptions
```shell
apropos manual
```

## Info Pages
### Generic: Info Page for command
```shell
info <command>
```

#### Example: Info Page for info
```shell
info info
```
### Navigating an open Info Page
#### Basic Info Page Commands
```shell
info <command>
```
Then once in info page press H on keyboad

#### Info Page tutorial
```shell
info <command>
```
Then once in info page press h on keyboad (if already on info Info page no change happends)

#### Exit Info Page
```shell
info <command>
```
To exit openned manual entry press q on keyboard

## Regex in Man & Info Pages
### Example: Search forward for string 'manual'
In an open Man or Info Page on the keyboard press / then type manual then press enter

### Example: Search backward for string 'manual'
In an open Man or Info Page on the keyboard press ? then type manual then press enter

### Generic: Next appearance of a string
Once used regex to search for a string navigate to the next appearance of the string by on the keyboard pressing n 

### Generic: Previous appearance of a string
Once used regex to search for a string navigate to the next appearance of the string by on the keyboard pressing N

# References and Guides
[GNU-Bash Reference Manual-Help](https://www.gnu.org/savannah-checkouts/gnu/bash/manual/bash.html#help)

[GNU-Manual-Man Pages](https://www.gnu.org/software/groff/manual/html_node/man.html)

[GNU-Manual-Regular Expressions](https://www.gnu.org/software/grep/manual/html_node/Regular-Expressions.html)

[GNU-Manual-Shell Builtin Commands](https://www.gnu.org/software/bash/manual/html_node/Shell-Builtin-Commands.html)

[GNU-Standards-Man Pages](https://www.gnu.org/prep/standards/html_node/Man-Pages.html)

[GNU-Standards-Help](https://www.gnu.org/prep/standards/html_node/_002d_002dhelp.html#g_t_002d_002dhelp)

[SS64](https://ss64.com/)