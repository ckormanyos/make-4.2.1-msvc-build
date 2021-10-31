# make-4.2.1-msvc-build

This repository takes the source code for GNUmake 4.2.1
within the file `make-4.2.1.tar.gz`
from [here](https://ftp.gnu.org/gnu/make/)
and adapts the legacy MSVC build to a more modern version of MSVC 14.2.

# Instructions to build make-4.2.1-msvc-build

Here are the instructions to build make-4.2.1-msvc-build.
  - Clone `make-4.2.1-msvc-build`
  - Navigate to the [MSVC solution file `make-4.2.1.sln` stored here](./make-4.2.1/)
  - Open `make-4.2.1.sln` in MSVC 14.2 --- i.e., Microsoft(R) VisualStudio(R) 2019 or higher, Community Edition works also.
  - Select Debug/Release as desired in the usual way.
  - Select x86 or x64 as desired in the usual way.
  - Rebuild solution and find the build artifacts including `make-4.2.1.exe` in the standard output path location(s).

You might want to rename the executable file to `make.exe`. Use this just like you wouls use `make` on `*nix`.
