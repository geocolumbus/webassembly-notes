# Web Assembly

## Usage

```
git clone https://github.com/geocolumbus/webassembly-notes.git
mv webassembly-notes hello
cd hello
```

### Compile
```
$ emcc hello.c -s WASM=1 -o hello.html
```

or

```
./compile
```

### Clean

```
./clean
```

### Serve

To serve the compiled files over HTTP, we can use the emrun web server provided with the Emscripten SDK:

```
$ emrun --no_browser --port 8080 .
```

## Assumes you have web assembly installed

https://webassembly.org/getting-started/developers-guide/

## WABT - tools for working with Web Assembly

| WABT Command | Description | man page link |
|-----------------|---------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------|
| spectest-interp | read a Spectest JSON file, and run its tests in the interpreter | https://www.mankier.com/1/spectest-interp |
| wasm-interp | decode and run a WebAssembly binary file | https://www.mankier.com/1/wasm-interp |
| wasm-objdump | print information about a wasm binary | https://www.mankier.com/1/wasm-objdump |
| wasm-opcodecnt | count opcode usage for instructions | https://www.mankier.com/1/wasm-opcodecnt |
| wasm-strip | remove sections of a WebAssembly binary file | https://www.mankier.com/1/wasm-strip |
| wasm-validate | validate a file in the WebAssembly binary format | https://www.mankier.com/1/wasm-validate |
| wasm2c | convert a WebAssembly binary file to a C source and header | https://www.mankier.com/1/wasm2c |
| wasm2wat | translate from the binary format to the text format | https://www.mankier.com/1/wasm2wat |
| wast2json | convert a file in the wasm spec test format to a JSON file and associated wasm binary files | https://www.mankier.com/1/wast2json |
| wat-desugar | parses .wat text form as supported by the spec interpreter (s-expressions, flat syntax, or mixed) and prints "canonical" flat format. | https://www.mankier.com/1/wat-desugar |
| wat2wasm | translate from WebAssembly text format to the WebAssembly binary format | https://www.mankier.com/1/wat2wasm |

