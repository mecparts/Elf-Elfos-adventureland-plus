# Elf/OS port of Richard Goedeken's 1802 Adventureland+

One quiet evening earlier this month, I did a quick and dirty port of
[Richard Goedeken's 1802 version of 
Adventureland](https://github.com/richard42/1802-adventureland-plus)
to run under Elf/OS. This is the result.

It includes Lee Hart's splash screen because, well, it's just so cool!

This version assumes an ANSI terminal.

The save/restore game functionality uses a disk file rather than upper
memory (/bin/adven-1.dat if you're curious where it ends up).


- adventureland.032 runs under Elf/OS 0.3.2 (it saves the game in the
  /BIN/ directory rather than /bin/)
- adventureland.040 runs under Elf/OS 0.4.0 (it uses /bin/)

The source was assembled with my extended, tweaked and customised
version of the a18 1802 assembler.

## Minor game enhancement

After discovering that if I climbed the cypress tree, got the keys,
came back down and then dropped the keys that I was unable to chop the
tree down, I included one additional command handler that wasn't in the
original source. It just bugged me.

