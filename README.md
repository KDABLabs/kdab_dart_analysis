# KDAB analysis

Analysis options used for Dart and Flutter at KDAB.
This repo is heavily inspired by [very_good_analysis](https://pub.dev/packages/very_good_analysis).

## Usage

Add add a dev dependency for dart projects:
```bash
dart pub add dev:kdab_dart_analysis
```

Add add a dev dependency for flutter projects:
```bash
flutter pub add dev:kdab_dart_analysis
```

Then include in `analysis_options.yaml`
```yaml
include: package:kdab_dart_analysis/analysis_options.yaml
```

To use a specific version use:
```yaml
include: package:kdab_dart_analysis/analysis_options_1.0.0.yaml
```

## Additional information

### Suppressing lints

You can suppress specific lints for the project by adding it to your `analysis_options.yaml`
```yaml
include: package:kdab_dart_analysis/analysis_options.yaml
linter:
  rules:
    public_member_api_docs: false
```