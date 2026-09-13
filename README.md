# purs-orm

## Overview

生成される SQL が予測可能で一意に定まる、PureScript の ORM。

pre-alpha。設計中で、実装はまだない。

## Features

実装済みの機能はまだない。

## Prerequisites

- Nix (flakes 有効)
- direnv
- 対応システムは `x86_64-linux` のみ

## Usage

```sh
direnv allow
```

## Directory Structure

```
.
├── docs/
│   └── DESIGN.md    設計方針
├── nix/             flake-parts の各モジュール
├── src/
│   └── Main.purs
└── test/
    └── Main.purs
```
