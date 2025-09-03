make-4.2.1-msvc-build
==================

[![Build Status](https://github.com/ckormanyos/make-4.2.1-msvc-build/actions/workflows/make-4.2.1.yml/badge.svg)](https://github.com/ckormanyos/make-4.2.1-msvc-build/actions)

This repository takes the source code for GNUmake 4.2.1
within the file `make-4.2.1.tar.gz`
from [here](https://ftp.gnu.org/gnu/make/)
and adapts the legacy MSVC build to a more modern version of MSVC 14.2.

# Instructions to build make-4.2.1-msvc-build

Here are the instructions to build make-4.2.1-msvc-build.
  - Clone or get [ckormanyos/make-4.2.1-msvc-build](https://github.com/ckormanyos/make-4.2.1-msvc-build).
  - Navigate to the MSVC solution file `make-4.2.1.sln` which is [stored here](./make-4.2.1/).
  - Open `make-4.2.1.sln` in MSVC 14.2 - i.e., Microsoft(R) VisualStudio(R) 2019 or higher (the Community Edition works also).
  - Select Debug/Release as desired in the usual way.
  - Leave the solution configuration `x64` set in the usual way (since this is actually the only supported solution configuration).
  - Rebuild solution and find the executable file `make-4.2.1.exe` in the standard output path location.

You might want to rename the executable from `make-4.2.1.exe` file to simply `make.exe`.
The resulting executable file `make-4.2.1.exe` ( or if manually renamed `make.exe`)
can be used just like you would use regular, traditional `make` on `*nix`.

# Changes

Minor changes in the source code have been undertaken.
  - Disable the famous warning 4996.
  - Leave all other warnings unchanged.
  - Change the name of one _shadowed_ variable.
  - Update the legacy MSVC workspace and adapt its naming.
  - Add a solution configuration `x64` with settings initially copied from `x86` in the usual _MSVC_ way.
  - Eliminate the `x86` configuration and retain only the 64-bit solution configuration `x64`.
  - Upload build artifact in CI for `make-4.2.1-win64-msvc`, see also discussion in [issue 1](https://github.com/ckormanyos/make-4.2.1-msvc-build/issues/1).
  - Add `TCC`-support (from @jamosdev). `TCC` is the tiny C-Compiler, which is a very efficient and portable standalone C-Compiler. For further information, please see the discussion in [pr 10 ](https://github.com/ckormanyos/make-4.2.1-msvc-build/pull/10)
