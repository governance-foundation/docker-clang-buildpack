# Clang Build Pack

[![build_status](https://github.com/governance-foundation/docker-clang-buildpack/workflows/ci/badge.svg?branch=ubuntu-10)](https://github.com/governance-foundation/docker-clang-buildpack/actions?query=workflow%3Aci)
[![github license](https://img.shields.io/github/license/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github issues](https://img.shields.io/github/issues/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github last commit](https://img.shields.io/github/last-commit/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![github repo size](https://img.shields.io/github/repo-size/governance-foundation/docker-clang-buildpack)](https://github.com/governance-foundation/docker-clang-buildpack)
[![docker stars](https://img.shields.io/docker/stars/gvfn/clang-buildpack)](https://hub.docker.com/r/gvfn/clang-buildpack)
[![docker pulls](https://img.shields.io/docker/pulls/gvfn/clang-buildpack)](https://hub.docker.com/r/gvfn/clang-buildpack)

This is docker image with [LLVM/Clang](https://llvm.org/) and [Boost](https://www.boost.org/)

## Included Packages

Following is the list of packages included

* llvm 10 using [https://chocolatey.org/packages/llvm](https://chocolatey.org/packages/llvm)
* python 3 [https://chocolatey.org/packages/python](https://chocolatey.org/packages/python)
* vcpkg [https://github.com/Microsoft/vcpkg](https://github.com/Microsoft/vcpkg)
* Lib: Boost `vcpkg install boost:x64-windows`
* Lib: Curl `vcpkg install curl:x64-windows`

## Running

Run this command from your project folder:

In Powershell:

```powershell
docker run -it --rm -v ${pwd}:/build gvfn/clang-buildpack:windows cmd.exe
```

In Bash

```powershell
docker run -it --rm -v `pwd`:/build gvfn/clang-buildpack:windows cmd.exe
```

Your current folder will be mapped into `/build` folder for your build activities.
