# helloworld

<https://zerolang.ai/getting-started>

```sh
cd helloworld
zero init
```

## Usage

```sh
zero run

zero view --fn main

zero query --fn main
zero query --calls write
zero query --find hello

zero export
```

## Helloworld

`zero query --fn main` shows the `main` function summary (signature, calls, and handles).

```sh
zero query --fn main
query: fn:main
module: package:helloworld@0.1.0 hash: graph:d4680751c158be5e

functions:
  main(world: World) -> Void raises #fn_main body:#block_main_body
    calls:
      world.out.write -> #param_main_world

tip: add --handles to list stmt and param patch handles; patch ops: zero patch --op help
```

`zero patch --replace-in-fn ...` edits `main` directly in this package (run it in `helloworld`).

```sh
zero patch --replace-in-fn main --old 'hello from zero\n' --new 'hello world from zero\n'
```

`zero run -- 40 2` runs with args. If the program does not read args, they have no effect.

```sh
zero run -- 40 2
hello world from zero
```
