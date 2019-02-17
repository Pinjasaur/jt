# jt

[![Travis](https://img.shields.io/travis/Pinjasaur/jt.svg)](https://travis-ci.org/Pinjasaur/jt)

Jot down notes. A simplified version of [`jot`][jot], requested by [@davidmerfield][david].

Creates timestamped files to rapidly jot down notes from the CLI.

## Installation

Add the [`jt` script](/jt) to your `$PATH` or create a function similar to:

```bash
jt() { 
  bash /path/to/jt "${@}" 
}
```

`jt` defaults to writing to `$HOME/Notes`. You can customize this by setting
`$JT_DIR` to something else (e.g. `export JT_DIR="$HOME/Dropbox/Notes"`).

You'll also want to make sure `$EDITOR` is set to your preferred editor 
(e.g. `export EDITOR='vim'`).

## Usage

```
jt [<arguments>]

  Creates a file in $JT_DIR/YYYY-mm-dd-HH:MM:SS.txt.

Options:
  -h --help  Show this.
  <data>     Populate file with <data>. If not set, open file with $EDITOR.
```

## License

[MIT][license] &copy; Paul Esch-Laurent.

[license]: https://pinjasaur.mit-license.org/2019
[david]: https://github.com/davidmerfield
[jot]: https://github.com/Pinjasaur/jot
