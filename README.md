# Stout

`stout` is a small utility written in perl that allow a program to write to stdout while having a permanent status line at the bottom.

Very useful when you have a script chaining several programs that writes a lot of things to stdout and you want to keep track of what is currently executing.

## Usage

```
Usage:  some_command_that_writes_to_stdout | stout <message>
```

## Example

```
$ ping localhost | stout "Pinging localhost"
PING localhost (127.0.0.1) 56(84) bytes of data.
64 bytes from localhost (127.0.0.1): icmp_seq=1 ttl=64 time=0.052 ms
64 bytes from localhost (127.0.0.1): icmp_seq=2 ttl=64 time=0.070 ms
64 bytes from localhost (127.0.0.1): icmp_seq=3 ttl=64 time=0.070 ms
...
[more lines will be written here]
...
Pinging localhost
```

## License

This script is released under the terms of the MIT License. See the LICENSE.txt file for more details.