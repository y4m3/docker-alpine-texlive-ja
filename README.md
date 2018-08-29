# y4m3/alpine-texlive-ja

> Minimal TeX Live image for Japanese based on alpine with Noto Sans/Serif CJK.

Forked from [Paperist/docker-alpine-texlive-ja] \(under the MIT License\).

## Table of Contents

- [Feature](#feature)
- [Install](#install)
- [Usage](#usage)
- [Contribute](#contribute)
- [License](#license)

## Feature

- Lightweight Docker image (alpine based)
- Japanese LaTeX environment with [Noto Sans/Serif CJK JP](https://www.google.com/get/noto/).

## Install

```bash
docker pull y4m3/alpine-texlive-ja
```

## Usage

### Basic use

```bash
$ docker run --rm -it -v $PWD:/workdir y4m3/alpine-texlive-ja
$ latexmk -C main.tex && latexmk main.tex && latexmk -c main.tex
```

### Use latexmk

set [y4m3/alpine-texlive-ja/.latexmkrc]()

```bash
$ docker run --rm -it -w=/workdir -v $PWD:/workdir y4m3/alpine-texlive-ja /bin/bash -c 'latexmk -pvc main.tex'
```

## Contribute

PRs accepted.

## License

MIT © y4m3

