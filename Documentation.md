# Documentation
## man <command>: Displays the manual page (documentation) for a specific command. (e.g., man ls)

## whatis <command>: Provides a brief, one-line description of a command from its manual page.

## man -f <command>: Exactly identical to whatis; looks up the short description.

## apropos <keyword> or man -k <keyword>: Searches the manual page names and descriptions for a specific keyword.

## info <command>: Displays more detailed, hyperlinked GNU info documents for a command compared to man.

# Where to get help documentation:

## <command> --help or <command> -h for quick inline usage flags.

## /usr/share/doc/ directory for package-specific READMEs and guides.

# Online resources like tldr pages (community-driven simplified man pages).

# 2. Searching & History
## find <path> <expression>: Searches for files and directories in a directory hierarchy based on criteria like name, size, or modification time. (e.g., find /home/user -name "*.txt")

## locate <filename>: Quickly finds files by name using a prebuilt database (faster than find, but relies on an updated index via updatedb).

## history: Displays the list of previously executed commands in your current shell session.

# 3. Control Operators & Shell Expansion
## && (AND operator): Executes the second command only if the first command succeeds (exit status 0). (e.g., make && make install)

## || (OR operator): Executes the second command only if the first command fails (non-zero exit status). (e.g., grep "test" file.txt || echo "Not found")

## ; (Semicolon): Separates multiple commands to be executed sequentially, regardless of success or failure. (e.g., cd /tmp; ls)

## !1 (History expansion): Runs command number 1 from your command history list. (!<number> repeats that specific command).

## Double Quotes ("..."): Interpolates variables and command substitutions while preserving spaces, but prevents wildcard expansion (globbing).

Backquotes (`...`) or $(...) (Command substitution): Executes the enclosed command and substitutes its output into the surrounding command. (e.g., echo "Today is $(date)")

4. Environment & Variables
To display the value of a variable: Precede the variable name with a dollar sign $. (e.g., echo $USER)

env: Prints all exported environment variables currently set in the session.

export <VAR>=<value>: Sets an environment variable so it is available to child processes and scripts. (e.g., export EDITOR=nano)

unset <VAR>: Removes (deletes) a shell variable or environment variable.

PATH: A special environment variable ($PATH) containing a colon-separated list of directories where the shell looks for executable programs.

5. Command Location & Inspection
type <command>: Indicates how a given command will be interpreted by the shell (whether it's a builtin, keyword, alias, or external file).

which <command>: Locates the executable file associated with a given command by searching the $PATH directories.

6. Customization & Flow Control
alias <name>='<command>': Creates a shortcut or custom name for a command or command sequence. (e.g., alias ll='ls -la')

unalias <name>: Removes an existing command alias.

Functions: Reusable blocks of shell commands defined in your script or shell configuration.

Bash
my_func() {
    echo "Hello $1"
}
| (Pipe operator): Redirects the standard output of the command on the left as the standard input to the command on the right. (e.g., cat file.txt | grep "error")

What specific command or workflow would you like to explore or practice next?
