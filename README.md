# SwiftCov

Super early tool (read: not working) to generate test code coverage information
for Swift.

## Usage

```shell
$ swiftcov generate [swiftcov options] xcodebuild [xcodebuild options]
```

### Example

```shell
$ swiftcov generate xcodebuild -project Example.xcodeproj -scheme 'Example' -configuration Release -sdk iphonesimulator test
```

```shell
$ swiftcov generate --output ./coverage --threshold 1 xcodebuild -project Example.xcodeproj -scheme 'Example' -configuration Release -sdk iphonesimulator test
```

__`-configuration` option and `-sdk` option in xcodebuild command must be specified.__

### Options

- `--output` specify output directory for generated coverage files
- `--threshold` specify limitation for counting hit count (for performance)

## License

MIT licensed.
