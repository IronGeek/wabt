<h1><p align="center" style="font-size:1.5rem;font-weight:normal"><img src="https://github.com/WebAssembly/web-assembly-logo/raw/master/dist/logo/web-assembly-logo-256px.png" alt="webassembly" /><br />Binary Toolkit (WABT) Installation via NPM</p></h1>

[![npm](https://img.shields.io/npm/v/@irongeek/wabt?logo=npm)](https://www.npmjs.com/package/@irongeek/wabt)
[![npm downloads](https://img.shields.io/npm/dt/@irongeek/wabt?logo=npm)](https://www.npmjs.com/package/@irongeek/wabt)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/IronGeek/wabt?logo=github)](https://github.com/IronGeek/wabt/releases)
[![GitHub issues](https://img.shields.io/github/issues/IronGeek/wabt?logo=github)](https://github.com/IronGeek/wabt/issues)
[![License](https://img.shields.io/github/license/IronGeek/wabt)](https://github.com/IronGeek/wabt/blob/master/LICENSE)

This package will download, compile, and install the [WebAssembly](https://webassembly.org) Binary Toolkit (WABT) from https://github.com/WebAssembly/wabt as [NPM](https://www.npmjs.com) global executables.  

## Prerequisites

- [git](https://git-scm.com/)
- [cmake](https://cmake.org/)
- make 

## Installation

``` sh
npm install -g @irongeek/wabt
```
> 📌 **NOTE**
> 
> Please give it some time to finish... 🙏
>
> _Depends on your computer specs, the installation process might take a while, and because NPM suppresses all output from custom install script (_unless exception is thrown_), the process might seems like it's stuck or hanging while it's actually busy compiling the binaries._

## Included Tools

| Tools | Description |
| ----- | ----------- |
| [`wat2wasm`][wat2wasm] | translate from WebAssembly text format to the WebAssembly binary format |
| [`wasm2wat`][wasm2wat] | the inverse of `wat2wasm`, translate from the binary format back to the text format (also known as a `.wat`) |
| [`wasm-objdump`][wasm-objdump] | print information about a wasm binary. Similiar to objdump |
| [`wasm-interp`][wasm-interp] | decode and run a WebAssembly binary file using a stack-based interpreter |
| [`wasm-decompile`][wasm-decompile] | decompile a wasm binary into readable C-like syntax |
| [`wat-desugar`][wat-desugar] | parse `.wat` text form as supported by the spec interpreter (s-expressions, flat syntax, or mixed) and print _canonical_ flat format |
| [`wasm2c`][wasm2c] | convert a WebAssembly binary file to a C source and header |
| [`wasm-strip`][wasm-strip] | remove sections of a WebAssembly binary file |
| [`wasm-validate`][wasm-validate] | validate a file in the WebAssembly binary format |
| [`wast2json`][wast2json] | convert a file in the wasm spec test format to a JSON file and associated wasm binary files |
| [`wasm-opcodecnt`][wasm-opcodecnt] | count opcode usage for instructions |
| [`spectest-interp`][spectest-interp] | read a Spectest JSON file, and run its tests in the interpreter |

## Known Issues

Must be run under bourne shell (`sh`) compatible terminal.

>  _May or may not work on Windows using [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl)_.

## Acknowledgement

Mathias Buus for the original [webassembly-binary-toolkit](https://github.com/mafintosh/webassembly-binary-toolkit.git) installation script.

## License

This package is released under the terms of [The MIT License](https://github.com/IronGeek/wabt/blob/master/LICENSE)

[wat2wasm]: https://webassembly.github.io/wabt/doc/wat2wasm.1.html
[wasm2wat]: https://webassembly.github.io/wabt/doc/wasm2wat.1.html
[wasm-objdump]: https://webassembly.github.io/wabt/doc/wasm-objdump.1.html
[wasm-interp]: https://webassembly.github.io/wabt/doc/wasm-interp.1.html
[wasm-decompile]: https://webassembly.github.io/wabt/doc/wasm-decompile.1.html
[wat-desugar]: https://webassembly.github.io/wabt/doc/wat-desugar.1.html
[wasm2c]: https://webassembly.github.io/wabt/doc/wasm2c.1.html
[wasm-strip]: https://webassembly.github.io/wabt/doc/wasm-strip.1.html
[wasm-validate]: https://webassembly.github.io/wabt/doc/wasm-validate.1.html
[wast2json]: https://webassembly.github.io/wabt/doc/wast2json.1.html
[wasm-opcodecnt]: https://webassembly.github.io/wabt/doc/wasm-opcodecnt.1.html
[spectest-interp]: https://webassembly.github.io/wabt/doc/spectest-interp.1.html
