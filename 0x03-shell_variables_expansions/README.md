# SHELL VARIEBLE EXPANSION
When the shell receives a command, either from the user typing at the keyboard, or from a shell script, it breaks it up into words. After this happens, the shell performs seven operations on the words, which can change how they are interpreted. These seven operations are collectively known as 'shell expansion'. You are probably familiar with most of them as we have used them throughout this book.

The seven operations that the shell performs are:

Brace Expansion - expanding values between braces, such as `file{1..3}` into `file1 file2 file3`
Tilde Expansion - expanding the ` ~ ` tilde symbol for the home directory into the path to the home directory, such as ` ~/effective-shell ` into ` /home/dwmkerr/effective-shell `
Parameter Expansion - expanding terms that start with a ` $ ` symbol into parameter values, such as ` $HOME ` into the value of the variable named ` HOME `
Command Substitution - evaluation of the contents of ` $(command) ` sequences, which are used to run commands and return the results to the shell command line
Arithmetic Expansion - evaluation of the contents of ` $((expression)) ` sequences, which are used to perform basic mathematical operations
Word Splitting - once all of the previous operations are run, the shell splits the command up into 'words', which are the units of text that you can run loops over
Pathname Expansion - the shell expands wildcards and special characters in pathnames, such as ``file*.txt`` into the set of files that are matched by the sequence
