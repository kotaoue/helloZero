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
