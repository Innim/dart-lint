# innim_lint

[![pub package](https://img.shields.io/pub/v/innim_lint)](https://pub.dartlang.org/packages/innim_lint)
[![Analyze & Test](https://github.com/Innim/dart-lint/actions/workflows/dart.yml/badge.svg?branch=main)](https://github.com/Innim/dart-lint/actions/workflows/dart.yml)

This package contains analysis settings for Flutter/Dart projects and packages by [Innim team](https://github.com/innim/).

It's stricter than [pedantic](https://pub.dev/packages/pedantic).

See [Customizing static analysis](https://dart.dev/guides/language/analysis-options#enabling-linter-rules).

## Usage

To use the lints add a dependency in your `pubspec.yaml`:

```yaml
# If you use `unawaited()` in code, add a normal dependency.
dependencies:
  innim_lint: ^0.3.1

# Or, if you just want `analysis_options.yaml`, it can be a dev dependency.
dev_dependencies:
  innim_lint: ^0.3.1
```

then, add an include in your `analysis_options.yaml`:

```yaml
include: package:innim_lint/analysis_options.yaml
```

### Unawaited 

Not all futures need to be awaited. By default "unawaited futures" lint enabled
which enforces that potential futures in asynchronous functions are handled somehow. 
If a particular future value doesn't need to be awaited, you can call `unawaited(...)` with it, 
which will avoid the lint, simply because the expression no longer has type Future. 

Function [`unawaited`](https://api.dart.dev/stable/2.16.0/dart-async/unawaited.html)
appeared in [`dart:async`](https://api.dart.dev/stable/2.16.0/dart-async/dart-async-library.html)
since 2.15.

### Disable some rules

You can disable some rules in your project. Add in your `analysis_options.yaml`:

```yaml
linter:
  rules:
    prefer_single_quotes: false
```

### Exclude from analysis

You can exclude some files from analysis - see [Excluding code from analysis](https://dart.dev/guides/language/analysis-options#excluding-files).

By default all generated code (files with `.g.dart` suffix) will be excluded with this analysis settings. 