# innim_lint

[![pub package](https://img.shields.io/pub/v/innim_lint)](https://pub.dartlang.org/packages/innim_lint)

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

### Disable some rules

You can disable some rules in your project. Add in your `analysis_options.yaml`:

```yaml
linter:
  rules:
    prefer_single_quotes: false
```

### Exclude from analysis

You can exculde some files from analysis - see [Excluding code from analysis](https://dart.dev/guides/language/analysis-options#excluding-files).

By default all generated code (files with `.g.dart` suffix) will be excluded with this analysis settings. 