# Developer Guide

## Commands

- `nix fmt` - Format code
- `nix flake check` - Run checks (format, lint, tests)
- `nix build` - Build the executable into `result/bin/app`
- `nix run` - Build and run the executable
- `purs-nix compile` - Generate `output/` for editor/LSP use
- `purs-nix run` - Compile and run `Main.main` with Node.js
- `purs-nix test` - Compile and run `Test.Main.main` with Node.js

## Notes

- `app` (`nix build` / `nix run` で得られる `result/bin/app`) はテンプレート由来の暫定物で、ライブラリ本体ではない
- `*.purs` は pre-commit の treefmt フックから除外されている (`nix/pre-commit.nix`) ため、PureScript の整形は `nix fmt` を明示的に実行する必要がある
- 依存の追加や変更は `spago.yaml` ではなく `nix/packages.nix` の `dependencies` / `test-dependencies` を編集する
