# TrailTrueBypass

[![KiBot](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml)
[![Doxygen](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/doxygen.yml/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/doxygen.yml)
[![pages-build-deployment](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/pages/pages-build-deployment)

[![XC8 - 3.10](https://img.shields.io/static/v1?label=XC8&message=3.10&color=red)](https://www.microchip.com/en-us/tools-resources/develop/mplab-xc-compilers)
[![KiCad](https://img.shields.io/badge/-314CB0?style=flat&logo=kicad&logoSize=auto)](https://downloads.kicad.org/kicad/windows/explore/stable)
[![MIT](https://img.shields.io/badge/License-MIT-green)](/LICENSE)

8ピンのPICマイコンでトレイルバイパスを実装するための基板とソースコードです。

## Features

- Normal true bypass when Trail mode off
- Selectable operating mode: Alternate or Momentary
- Set the power-on state: ON or OFF
- (Option) Selectable timing to switch: when-pressed or when-released
- Automatically bypasses if power is accidentally turned off

## Verified on

- PIC12F629
- PIC12F675

---

Coming soon?

- PIC12F1822
- PIC16F15313

## dir: KiCad

KiCad関連のファイル一式です。

ガーバーファイルは[Release](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/releases)からダウンロードできます。

## dir: src

PICマイコン用のソースコード群です。

プロジェクト管理の様式はVScode用のMPLAB Extension Packに準拠しています。

コンパイル後のhexファイルは[Release](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/releases)からダウンロードできます。

PICマイコン間で共通のソースコードはsrc直下に、そうでないものはそのハードウェアの名前の付いたディレクトリに入っています。

src/header.hの冒頭で所望のPICマイコンのヘッダーファイルをincludeするだけで、そのPICマイコンが書き込み対象となります。
