<h1 align="center">
TrailTrueBypass_PIC
</h1>

<div align="center">

**A project for a trail-bypass with an DIP8 PIC microcontroller.**

[![KiBot](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/kibot.yml)
[![Format code](https://github.com/asumo-1xts/TrailTrueBypass_PIC/actions/workflows/format.yml/badge.svg)](https://github.com/asumo-1xts/TrailTrueBypass_PIC/actions/workflows/format.yml)
[![Doxygen](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/doxygen.yml/badge.svg)](https://github.com/aSumo-1xts/TrailTrueBypass_PIC/actions/workflows/doxygen.yml)

[![XC8 - 3.10](https://img.shields.io/static/v1?label=XC8&message=v3.10)](https://www.microchip.com/en-us/tools-resources/develop/mplab-xc-compilers)
[![KiCad](https://img.shields.io/badge/v8-314CB0?logo=kicad&logoSize=auto&labelColor=gray)](https://downloads.kicad.org/kicad/windows/explore/stable)
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

PICマイコン間で共通のソースコードはsrc直下に、そうでないものはそのハードウェアの名前の付いたディレクトリに入っています。

src/header.hの冒頭で所望のPICマイコンのヘッダーファイルをincludeするだけで、そのPICマイコンが書き込み対象となります。
