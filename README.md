# innim_lint

[![pub package](https://img.shields.io/pub/v/list_ext)](https://pub.dartlang.org/packages/innim_lint)

This package contains analysis settings for Flutter/Dart projects and packages by [Innim team](https://github.com/innim/).

It's stricter than [pedantic](https://pub.dev/packages/pedantic).

See [Customizing static analysis](https://dart.dev/guides/language/analysis-options#enabling-linter-rules).

## Usage

To use the lints add a dependency in your `pubspec.yaml`:

```yaml
# If you use `unawaited()` in code, add a normal dependency.
dependencies:
  innim_lint: ^1.0.0

# Or, if you just want `analysis_options.yaml`, it can be a dev dependency.
dev_dependencies:
  innim_lint: ^1.0.0
```

then, add an include in your `analysis_options.yaml`:

```yaml
include: package:innim_lint/analysis_options.yaml
```