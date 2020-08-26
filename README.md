### Usage

```bash
$ # genenrate a random file
$ dd if=/dev/urandom bs=1024 count=128 of=myfile
$ # build project
$ cargo build
$ # execute against random file
$ cat myfile| target/debug/pipeviewer > myfile2
131072
$ # check files are the same
$ diff myfile myfile2
```
