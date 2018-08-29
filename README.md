# y4m3/alpine-texlive-ja

[![Docker Automated build](https://img.shields.io/docker/automated/y4m3/alpine-texlive-ja.svg)](https://hub.docker.com/r/y4m3/alpine-texlive-ja/)
[![Docker Image Size](https://images.microbadger.com/badges/image/y4m3/alpine-texlive-ja.svg)](https://microbadger.com/images/y4m3/alpine-texlive-ja "Get your own image badge on microbadger.com")

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

