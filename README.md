# bod
objdump beautifier

## aim
`bod` (for Beautify ObjDump) colorizes objdump's output to make it more
readable

## supported targets

In the current version of `bod` the following targets are supported:
* elf32-littlearm
* elf32-tradlittlemips
* elf32-i386
* elf64-x86-64

# Installation

Download `bod` and put it in `/usr/local/bin`


# Usage

## Basic

Pipe `objdump`'s output to bod, for example with:

``` bash
objdump -d ./binary | bod
```

If needed, this output can itself be piped to `less` thanks to

``` bash
objdump -d ./binary | bod | less -R
```

## Main options

`bod` allows:
* to have a glance at what is in the code with `-l` or `--list`
* to look at the disassembly of a single function with `-f` or `--function`
