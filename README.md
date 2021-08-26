# 0x16. C - Simple Shell :shell:

![Alt Text](https://www.howtogeek.com/wp-content/uploads/2021/05/laptop-with-terminal-big.png?width=1198&trim=1,1&bg-color=000&pad=1,1)

## Description
simple_shell is a command line interpreter, or shell, in the tradition of the first Unix shell written by Ken Thompson in 1971. This shell is intentionally minimalistic, yet includes the basic functionality of a traditional Unix-like command line user interface. 
Standard functions and system calls employed in simple_shell include:
   `access, execve, exit, fork, free, fstat, getline, malloc, perror, signal, stat, wait, write.`

## Resources :bookmark_tabs:
- Unix shell
- Thompson Shell
- Ken Thompson
- man `sh`

### General Topics
- Who designed and implemented the original Unix operating system
- Who wrote the first version of the UNIX shell
- Who invented the B programming language (the direct predecessor to the C programming language)
- Who is Ken Thompson-
- How does a shell work
- What is a pid and a ppid
- How to manipulate the environment of the current process
- What is the difference between a function and a system call
- How to create processes
- What are the three prototypes of main
- How does the shell use the PATH to find the programs
- How to execute another program with the execve system call
- How to suspend the execution of a process until one of its children terminates
- What is EOF / “end-of-file”?

## File Structure :file_folder:
### List of allowed functions and system calls

   - `access` (man 2 access)
   - `chdir` (man 2 chdir)
   - `close` (man 2 close)
   - `closedir` (man 3 closedir)
   - `execve` (man 2 execve)
   - `exit` (man 3 exit)
   - `_exit` (man 2 _exit)
   - `fflush` (man 3 fflush)
   - `fork` (man 2 fork)
   - `free` (man 3 free)
   - `getcwd` (man 3 getcwd)
   - `getline` (man 3 getline)
   - `getpid` (man 2 getpid)
   - `isatty` (man 3 isatty)
   - `kill` (man 2 kill)
   - `malloc` (man 3 malloc)
   - `open` (man 2 open)
   - `opendir` (man 3 opendir)
   - `perror` (man 3 perror)
   - `read` (man 2 read)
   - `readdir` (man 3 readdir)
   - `signal` (man 2 signal)
   - `stat` (__xstat) (man 2 stat)
   - `lstat` (__lxstat) (man 2 lstat)
   - `fstat` (__fxstat) (man 2 fstat)
   - `strtok` (man 3 strtok)
   - `wait` (man 2 wait)
   - `waitpid` (man 2 waitpid)
   - `wait3` (man 2 wait3)
   - `wait4` (man 2 wait4)
   - `write` (man 2 write)

## Compilation

Your shell will be compiled this way:

```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh 
```

## Testing

The shell should work like this in interactive mode:
```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```


## Requirements

simple_shell is designed to run in the `Ubuntu 14.04 LTS` linux environment and to be compiled using the GNU compiler collection v. `gcc 4.8.4` with flags`-Wall, -Werror, -Wextra, and -pedantic.`

## Installation

   - Clone this repository: `git clone "https://github.com/winstoneochieng/simple_shell.git"`
   - Change directories into the repository: `cd simple_shell`
   - Compile: `gcc -Wall -Werror -Wextra -pedantic *.c -o hsh`
   - Run the shell in interactive mode: `./hsh`
   - Or run the shell in non-interactive mode: example `echo "pwd" | ./hsh`

## Bugs
At this time, there are no known bugs.

## Authors :black_nib:



| Authors     | Profile |
| ----------- | ----------- |
| Winstone Ochieng     | [Winstone Ochieng](https://www.winweb.cloudrebue.co.ke)      |
| Hewan Tegenie  | [Hewan Tegenie](https://github.com/Hewan2568)        |

## Acknowledgements :pray:


This project was written as part of the curriculum for ALX Software Engineering Program in partnership with Holberton School and it emulates basic functionality of the **sh** shell. Holberton School is a campus-based full-stack software engineering program that prepares students for careers in the tech industry using project-based peer learning. For more information, visit [this link](https://www.alxafrica.com/).

<p align="center">
  <img src="https://alx-apply.hbtn.io/brand_alx/share_image_2019.jpg" alt="ALX logo">
</p>