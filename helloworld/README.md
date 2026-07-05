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

```sh
zero patch /tmp/add-cli.patch

/tmp/add-cli.patch:1:1 BLD002: graph patch requires patch operations
  expected: one patch source: file, --op, --patch-text, --replace-fn, --replace-in-fn, or --rewrite
  actual: missing patch input
  help: pass a zero-program-graph-patch v1 file, one or more --op lines, --replace-fn with --body-file, or --replace-in-fn with --old and --new
  explain: zero explain BLD002
```

```sh
zero patch /tmp/add-cli.patch

/tmp/add-cli.patch:1:1 BLD002: graph patch requires patch operations
  expected: one patch source: file, --op, --patch-text, --replace-fn, --replace-in-fn, or --rewrite
  actual: missing patch input
  help: pass a zero-program-graph-patch v1 file, one or more --op lines, --replace-fn with --body-file, or --replace-in-fn with --old and --new
  explain: zero explain BLD002
```

```sh
zero run -- 40 2
hello world from zero
```
