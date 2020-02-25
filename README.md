
# SwiftFormatSample

[SwiftFormat](https://github.com/nicklockwood/SwiftFormat)の導入のサンプル。

このリポジトリは以下の環境で作った。

- macOS 10.15.3
- Xcode 11.3.1

## 手順

### Xcodeでプロジェクトを作る

### `BuildTools/Package.swift`を書く

```swift
// swift-tools-version:5.1
import PackageDescription

let package = Package(
    name: "BuildTools",
    platforms: [.macOS(.v10_11)],
    dependencies: [
        .package(url: "https://github.com/nicklockwood/SwiftFormat", from: "0.41.2"),
    ]
)
```

### Run Script

![Run Script](https://i.gyazo.com/3b877684d031bcf7d9fe4d5019aadf1d.png)]

## `.gitignore`

```.gitignore
# SwiftPM
BuildTools/.build
```

### ビルドする
