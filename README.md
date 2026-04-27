<div align="center">

<img src="https://socialify.git.ci/hxreborn/discover-ads-filter/image?description=1&font=Inter&logo=https%3A%2F%2Fraw.githubusercontent.com%2Fhxreborn%2Fdiscover-ads-filter%2Frefs%2Fheads%2Fmain%2Fartwork%2Ficon.png&name=1&pattern=Brick+Wall&theme=Auto" alt="discover-ads-filter" width="640" height="320" />

<p>An LSPosed module that hides sponsored cards and ad clusters from the Google Discover feed in the Pixel Launcher -1 screen and inside the Google app itself. Uses DexKit to dynamically resolve obfuscated targets.</p>

<br>

![AGSA 17.14+](https://img.shields.io/badge/AGSA-17.14%2B-4285F4?style=flat&logo=google&logoColor=white)
![libxposed API 101](https://img.shields.io/badge/libxposed-API_101-ff69b4?style=flat)
![DexKit 2.2.0](https://img.shields.io/badge/DexKit-2.2.0-E65100?style=flat)

</div>

## Requirements

- Android 11+
- LSPosed manager with libxposed API 101 support

## Installation

1. Download the APK from [Releases](https://github.com/hxreborn/discover-ads-filter/releases)

2. Enable the module in LSPosed.
3. Scope it to Google App (`com.google.android.googlequicksearchbox`).

## Usage

1. Open the app and run a scan.
2. Force stop Google App or reboot.
3. Run the scan again after each Google App update.

## How It Works

The app scans the installed Google App with DexKit, resolving hook targets via protobuf extension field numbers and type signatures, and stores the result in a versioned cache. The hooked process uses the cached targets to filter ad items from the Discover feed.

## License

<a href="https://github.com/hxreborn/discover-ads-filter/blob/main/LICENSE"><img src="https://raw.githubusercontent.com/hxreborn/discover-ads-filter/main/.github/assets/gplv3.svg" height="90" alt="GPLv3" /></a>

This project is licensed under the GNU General Public License v3.0. See [LICENSE](https://github.com/hxreborn/discover-ads-filter/blob/main/LICENSE) for details.
