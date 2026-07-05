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
zero export
vim src/main.0
zero import
zero check
```

## build

```sh
zero build --emit exe --target linux-musl-x64 --out .zero/out/app
./.zero/out/app 
zsh: exec format error: ./.zero/out/app
```
