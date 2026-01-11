<h1 align="center">

TrailTrueBypass_PIC

</h1>

<div align="center">

**A project for a trail-bypass with an DIP8 PIC microcontroller.**

[![KiBot](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml)
[![Format | Docs](https://github.com/asumo-1xts/TrailTrueBypass_PIC/actions/workflows/format-docs.yml/badge.svg)](https://github.com/asumo-1xts/TrailTrueBypass_PIC/actions/workflows/format-docs.yml)

[![KiCad](https://img.shields.io/badge/-%23314CB0?style=flat&logo=kicad&logoColor=white&logoSize=auto)](https://downloads.kicad.org/kicad/windows/explore/stable)
[![XC8](https://img.shields.io/badge/XC8-%23A8B9CC?style=flat&logo=c&logoColor=white)](https://www.microchip.com/en-us/tools-resources/develop/mplab-xc-compilers)
[![Clang-Format](https://img.shields.io/badge/Clang--Format-gray?style=flat)](https://clang.llvm.org/docs/ClangFormat.html)
[![Doxygen](https://img.shields.io/badge/-%232C4AA8?style=flat&logo=doxygen&logoColor=white&logoSize=auto)](https://www.doxygen.nl/)
[![MIT](https://img.shields.io/badge/License-MIT-green)](/LICENSE)

</div>

## Features

- Normal true bypass when Trail mode off
- Selectable operating mode: Alternate or Momentary
- Set the power-on state: ON or OFF
- (Option) Selectable timing to switch: when-pressed or when-released
- Automatically bypasses if power is accidentally turned off

## Verified on

- PIC12F629
- PIC12F675

## dir: KiCad

KiCad関連のファイル一式です。

ガーバーファイルは[Release](https://github.com/asumo-1xts/TrailTrueBypass_PIC/releases)からダウンロードできます。

## dir: src

PICマイコン用のソースコード群です。

プロジェクト管理の様式はVScode用のMPLAB Extension Packに準拠しています。

コンパイル後のhexファイルは[Release](https://github.com/asumo-1xts/TrailTrueBypass_PIC/releases)からダウンロードできます。

PICマイコン間で共通のソースコードは`src`直下に、そうでないものはそのハードウェアの名前の付いたディレクトリに入っています。

`src/header.h`の冒頭で所望のPICマイコンのヘッダーファイルをincludeするだけで、そのPICマイコンが書き込み対象となります。
