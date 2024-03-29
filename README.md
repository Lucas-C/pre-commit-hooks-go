:warning: 
:warning: Use the hook provided by [`checkmake`](https://github.com/mrtazz/checkmake#pre-commit-usage), as [the checkmake hook in this repo is no longer maintained](https://github.com/Lucas-C/pre-commit-hooks-go/issues/2#issuecomment-1112959641).

# `pre-commit-hooks-go`

Useful [pre-commit](http://pre-commit.com) hooks written in Go language.

Currently it only includes [mrtazz Makefile linter](https://github.com/mrtazz/checkmake).

Requires that you have `go` installed.

## Usage

```
-   repo: https://github.com/Lucas-C/pre-commit-hooks-go
    rev: v1.0.1
    hooks:
    -   id: checkmake
```

## Development

`checkmake.go` is simply a copy of `cmd/checkmake/main.go` in https://github.com/mrtazz/checkmake.

To update it:

    curl https://raw.githubusercontent.com/mrtazz/checkmake/master/cmd/checkmake/main.go -o checkmake.go

