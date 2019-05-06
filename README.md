# Web Assembly

## Usage

```
$ mkdir hello
$ cd hello
$ cat << EOF > hello.c
#include <stdio.h>
int main(int argc, char ** argv) {
  printf("Hello, world!\n");
}
EOF
$ emcc hello.c -s WASM=1 -o hello.html
```

To serve the compiled files over HTTP, we can use the emrun web server provided with the Emscripten SDK:

```
$ emrun --no_browser --port 8080 .
```

## Assumes you have web assembly installed

https://webassembly.org/getting-started/developers-guide/


