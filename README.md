# helloZero

Helloworld for [zerolang](https://zerolang.ai/)

## Installation

```sh
curl -fsSL https://zerolang.ai/install.sh | bash
export PATH="$HOME/.zero/bin:$PATH"
zero --version
```

## Usage

```sh
zero view --fn main

zero check
zero test
```

## Development

```sh
zero init --template cli
zero patch --op 'addMain'
zero export
vim src/main.0
zero import
zero check
zero test
zero run
```

### build

```sh
zero doctor

# Linux x64
zero build --emit exe --target linux-musl-x64 --out .zero/out/app

# Mac
zero build --emit exe --target darwin-arm64 --out .zero/out/app

./.zero/out/app
```

### Skills

```sh
zero skills
```

## Key Takeaways

- like Go, zeroLang seems possible to build from the same source code on both Linux and Mac is Good.
- .graph is binary, Managing binaries code as binaries doesn't play well with Git is not Good.
- The writing experience is similar to C or Rust. It’s not bad, but it’s not best.
