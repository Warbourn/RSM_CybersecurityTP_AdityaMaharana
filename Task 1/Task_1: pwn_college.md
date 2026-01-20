# Linux Command Line Research: Module Summaries

## Module: Hello Hackers
This introductory module establishes foundational terminal interaction through simple commands like whoami and hello. It emphasizes Linux's strict case sensitivity, where "Hello" and "hello" are distinct entities. The module explores command-line arguments using echo to demonstrate how the shell parses input into commands and data tokens. It introduces command history navigation via arrow keys, enabling efficient recall of complex instructions without re-typing, thereby minimizing syntax errors and accelerating workflow during iterative operations.

## Module: Pondering Paths
This module analyzes the Linux filesystem hierarchy structured from root directory (/). It distinguishes absolute paths from relative paths interpreted via current working directory (CWD). Users learn cd navigation, ~ as home directory shortcut, and special notations: . (current directory) and .. (parent directory). These mechanics enable precise targeting of files and binaries across nested filesystems, essential for advanced system administration without constant directory navigation.

## Module: Comprehending Commands
This module introduces essential data management tools: cat for reading files, grep for filtering datasets, and diff for comparing files line-by-line. It covers filesystem operations including touch, mkdir, mv, and rm, plus hidden files with dot prefixes. The module explores find for locating files by attributes and symbolic links (ln -s) for flexible data organization across volumes.

## Module: Digesting Documentation
This module fosters technical self-sufficiency through program documentation interpretation. It covers man pages for comprehensive manuals, --help flags for quick summaries, and navigating documentation with keyboard shortcuts and / search. Researchers learn to decipher usage patterns and distinguish between standalone binaries and shell builtins. Mastering these methods enables users to dynamically learn any tool by "reading the manual."

## Module: File Globbing
This module introduces globbing for pattern matching and bulk file manipulation. It details wildcards: * (any characters), ? (one character), and [] (character sets). Exclusionary globbing uses [^...] syntax. Tab completion automatically finishes partially typed filenames. These patterns enable filtering and processing hundreds of files with minimal keystrokes, essential for data-heavy environments.

## Module: Practicing Piping
This module examines I/O redirection and piping through standard streams: stdin, stdout, and stderr. It explains > for output redirection, >> for appending, and | for chaining commands. Advanced techniques include 2> for error redirection, 2>&1 for stream merging, and tee for simultaneous file-saving and piping. Process substitution enables sophisticated data flow between programs.

## Module: Perceiving Permissions
This module analyzes Linux's access control model governing files through user and group ownership. It covers chown, chgrp, and chmod for managing Read, Write, and Execute permissions across User, Group, and Others categories. The critical SUID bit allows users to execute programs with owner privileges, granting temporary administrative access without root passwords—a powerful but high-risk security tool.

## Module: Pondering PATH
This module investigates command execution through the PATH environment variable—a colon-separated directory list the shell searches for commands. Manipulating PATH can disrupt operations or enable "hijacking" by prepending custom script directories. The which command identifies exact binary paths. Understanding PATH is vital for troubleshooting installations and recognizing security implications in system-critical process execution.

## Module: Chaining Commands
This module explores command orchestration through logical operators: ; (sequential execution), && (execute on success), and || (execute on failure). It transitions to shell scripting with .sh files, introducing the Shebang (#!/bin/bash), positional arguments ($1, $2), and conditional logic using if/elif/else blocks. These techniques enable automated workflows with error handling and multi-stage logic.

## Module: Data Manipulation
This module focuses on text transformation tools: tr for character translation and case-swapping, head for file beginnings, cut for column extraction, and sort for organizing datasets. These "building blocks" combine through pipes to transform chaotic raw data into structured, filtered information. Strategic sorting can relocate hidden values from thousands of decoys, essential for data analysis and security auditing.

## Module: Processes and Jobs
This module covers process management using ps -ef for inspection and kill for termination via PID. Job control includes Ctrl-C (interrupt), Ctrl-Z (suspend), bg (background resume), and fg (foreground return). The & operator launches background processes. Exit codes via $? signal success or errors, providing critical diagnostic information for script automation and debugging workflows.

## Module: Untangling Users
This module explores multi-user architecture through su (substitute user) for identity switching and privilege escalation. It demonstrates password cracking using john (John the Ripper) against /etc/shadow hashes. The module introduces sudo (superuser do) as the modern standard, allowing authorized users to execute specific root-level commands using their own credentials, following least-privilege principles with audit trails.

## Module: Shell Variables
This module investigates shell environment variable management using $ prefix for access and NAME=VALUE syntax for assignment. It emphasizes case sensitivity and no-space requirements. The export command makes variables available to child processes. Command substitution $(...) stores command output in variables, while read enables interactive input, creating dynamic, responsive shell environments for configuration and scripting.