# Clang Build Pack

[![build_status](https://github.com/governance-foundation/docker-clang-buildpack/workflows/ci/badge.svg)](https://github.com/governance-foundation/docker-clang-buildpack/actions?workflow=ci)
[![github license](https://img.shields.io/github/license/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github issues](https://img.shields.io/github/issues/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github last commit](https://img.shields.io/github/last-commit/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github repo size](https://img.shields.io/github/repo-size/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![docker stars](https://img.shields.io/docker/stars/aemdesign/centos-java-buildpack)](https://hub.docker.com/r/aemdesign/centos-java-buildpack)
[![docker pulls](https://img.shields.io/docker/pulls/aemdesign/centos-java-buildpack)](https://hub.docker.com/r/aemdesign/centos-java-buildpack)
[![github release](https://img.shields.io/github/release/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)

This is docker image with [LLVM/Clang](https://llvm.org/) and [Boost](https://www.boost.org/)

## Included Packages

Following is the list of packages included

* llvm 10 using [https://apt.llvm.org/llvm.sh](https://apt.llvm.org/llvm.sh)
* python 3
* pyenv using [https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer](https://github.com/pyenv/pyenv-installer/raw/master/bin/pyenv-installer)
* Lib: Boost
* Lib: Curl

## Running

Run this command from your project folder:

In Powershell:

```powershell
docker run -it --rm -v ${pwd}:/build gvfn/clang-buildpack:ubuntu-10 bash
```

In Bash

```powershell
docker run -it --rm -v `pwd`:/build gvfn/clang-buildpack:ubuntu-10 bash
```
