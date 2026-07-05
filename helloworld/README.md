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
