# eb

## Version 1.2.0

Processes FILE(s) -- or *stdin* if no FILE given -- emitting text between begining and ending delimeter pairs; the delimeters may be indentical.
If only a begining delimeter is specified, then the ending delimeter is set to the same.
The delimeters *must* be the initial characters of a line; any whitespace causes the delimeter to be ignored.
The remainder of the delimeter line is ignored.
Delimeters can not be nested.

By default the begining and ending delimters are both set to ```

## Command Line

```
Extract Blocks of delimeted text
usage: eb [OPTION]... [FILE]...
options:
  -h, --help           display this help and exit
      --version        display version and exit
      --license        display license and exit
      --readme         display readme and exit
  -o, --output FILE    output to FILE
  -b, --begin TEXT     TEXT indicates begining of block
  -e, --end TEXT       TEXT indicates end of block
  -t, --tag TEXT       output only matching blocks tagged with text
  -l, --lines          output C style line directives
  -x, --extension EXT  append EXT to the file name in line directives
```

## Building

Uses [HOL](https://github.com/stytri/hol) and [defer](https://github.com/stytri/defer).

Compile with [m](https://github.com/stytri/m).

