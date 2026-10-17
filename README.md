# Kronos 5G RAN

5G NR RAN (gNodeB) Software for Evaluation, Development, and PoC

Kronos 5G RAN is a 5G NR Radio Access Network (gNodeB) software platform intended for evaluation, development, interoperability testing, and Local 5G / Private 5G PoC environments.

> The Kronos 5G RAN software package is distributed through GitHub Releases. `git clone` retrieves this repository and README, but does not download the release package.

## Download v0.1.0

You can download the current release directly from the links below:

* [Download kronos5gran.tar.gz](https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/kronos5gran.tar.gz)
* [Download SHA256SUMS](https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/SHA256SUMS)

On Linux, the release can also be downloaded from the command line:

```bash
wget https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/kronos5gran.tar.gz
wget https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/SHA256SUMS
```

Verify the integrity of the downloaded archive:

```bash
sha256sum -c SHA256SUMS
```

If verification succeeds:

```text
kronos5gran.tar.gz: OK
```

Extract the package:

```bash
tar xzf kronos5gran.tar.gz
```

[English](#english) | [日本語](#日本語)

---

## English

### Overview

Kronos 5G RAN provides a 5G NR gNodeB environment for evaluating and testing 5G SA networks.

The software is designed with consideration for the RAN architecture defined by 3GPP specifications and is intended for use in research, development, interoperability testing, and PoC environments.

It can be used together with [Kronos 5G Core](https://github.com/PrototypeDeveloper/kronos-5g-core) to build an end-to-end 5G SA test environment.

### Highlights

* 5G NR gNodeB software for 5G Standalone (SA) networks
* Designed with consideration for the RAN architecture defined by 3GPP specifications
* Band n79 (TDD) support
* SDR support: USRP B210
* Works with Kronos 5G Core
* Basic connectivity verified using a UE simulator
* Free Demo Mode available
* Suitable for 5G / Local 5G / Private 5G evaluation and PoC environments

### Feature Support

The following functionality is available in v0.1.0.

| Feature                          | Support Status | Validation Status              |
| -------------------------------- | -------------- | ------------------------------ |
| NR Band: n79 (TDD)               | Supported      | Verified with UE simulator     |
| Connection to Kronos 5G Core     | Supported      | Basic connectivity verified    |
| SDR: USRP B210                   | Beta           | Not yet validated              |
| Connectivity with commercial UEs | Beta           | Not yet validated              |

Beta functionality is provided for evaluation and development purposes and has not yet been fully validated in an end-to-end environment.

### Verified Connectivity

Basic connectivity has been verified with the following configuration:

```text
UE (simulator) ⇔ Kronos 5G RAN ⇔ Kronos 5G Core ⇔ DN
```

DN: Data Network

Connectivity with commercial UEs and over-the-air operation using SDR hardware are currently provided as beta features and have not yet been functionally validated.

### Demo Mode

A free Demo Mode is available for evaluation.

Demo Mode supports:

* Up to [2] UEs

This allows basic 5G RAN functionality to be evaluated without a paid license.

### Releases

Release packages are distributed through the Releases section of this repository.

Current public release:

**Kronos 5G RAN v0.1.0**

Release files:

```text
kronos5gran.tar.gz
SHA256SUMS
```

The integrity of the downloaded archive can be verified with:

```bash
sha256sum -c SHA256SUMS
```

> Note: The automatically generated GitHub `Source code (zip)` and `Source code (tar.gz)` archives do not contain the Kronos 5G RAN release package. Please use `kronos5gran.tar.gz` from the Release Assets.

### Project Status

Kronos 5G RAN is currently intended primarily for:

* Evaluation
* Development
* Testing
* Interoperability verification
* Proof of Concept (PoC)

Functionality and interoperability will continue to be expanded and validated in future releases.

### Disclaimer

Kronos 5G RAN is an independent implementation intended for evaluation, development, testing, and PoC purposes.

This project does not claim 3GPP certification or full conformance.

Beta functionality has not yet been fully validated and should be considered experimental.

Over-the-air transmission requires an appropriate radio license in your country or region. Users are responsible for complying with all applicable radio regulations.

---

## 日本語

### 概要

Kronos 5G RAN は、5G Standalone（SA）ネットワークの評価・開発・相互接続試験を目的とした5G NR RAN（gNodeB）ソフトウェアです。

ローカル5G / プライベート5Gを含む、研究・開発・検証・PoC環境での利用を想定しています。

3GPP仕様で定義されているRANの構成を考慮して設計されています。

[Kronos 5G Core](https://github.com/PrototypeDeveloper/kronos-5g-core) と組み合わせることで、End-to-Endの5G SA試験環境を構築できます。

### ダウンロード

Kronos 5G RANのソフトウェアパッケージは、GitHubの Releases から配布しています。

以下のリンクからv0.1.0を直接ダウンロードできます。

* [kronos5gran.tar.gz をダウンロード](https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/kronos5gran.tar.gz)
* [SHA256SUMS をダウンロード](https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/SHA256SUMS)

Linuxでは、以下のコマンドでもダウンロードできます。

```bash
wget https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/kronos5gran.tar.gz
wget https://github.com/PrototypeDeveloper/kronos-5g-ran/releases/download/v0.1.0/SHA256SUMS
```

ダウンロード後、SHA-256ハッシュを確認します。

```bash
sha256sum -c SHA256SUMS
```

正常な場合は以下のように表示されます。

```text
kronos5gran.tar.gz: OK
```

アーカイブを展開します。

```bash
tar xzf kronos5gran.tar.gz
```

### 主な特徴

* 5G Standalone（SA）ネットワーク向けの5G NR gNodeBソフトウェア
* 3GPP仕様で定義されているRANの構成を考慮した設計
* Band n79（TDD）に対応
* SDRとしてUSRP B210に対応
* Kronos 5G Coreと組み合わせて利用可能
* UEシミュレータを使用した基本的な接続を確認済み
* 無料で利用可能なDemo Modeを提供
* 5G / ローカル5G / プライベート5Gの評価・PoC環境で利用可能

### 機能対応状況

v0.1.0では以下の機能を提供しています。

| 機能                     | 対応状況 | 動作検証              |
| ---------------------- | ---- | ----------------- |
| NR Band：n79（TDD）       | 対応   | UEシミュレータで確認済み     |
| Kronos 5G Coreとの接続     | 対応   | 基本通信を確認済み         |
| SDR：USRP B210          | β版   | 未検証               |
| 市販UEとの接続               | β版   | 未検証               |

β版機能は評価・開発用途として提供しているものであり、End-to-End環境での完全な動作検証はまだ実施していません。

### 動作確認

以下の構成で基本通信を確認しています。

```text
UE (simulator) ⇔ Kronos 5G RAN ⇔ Kronos 5G Core ⇔ DN
```

DN：Data Network

市販UEとの接続、およびSDRハードウェアを使用した無線での動作についてはβ版機能として提供しており、機能動作検証はまだ実施していません。

### Demo Mode

評価用途として無料で利用できる Demo Mode を提供しています。

Demo Modeでは以下を利用できます。

* UE：最大[2]台

有料ライセンスなしで、基本的な5G RAN機能を評価できます。

### リリース

リリースパッケージは、本リポジトリの Releases から配布しています。

現在の公開リリース：

**Kronos 5G RAN v0.1.0**

リリースファイル：

```text
kronos5gran.tar.gz
SHA256SUMS
```

ダウンロードしたアーカイブの整合性は、以下のコマンドで確認できます。

```bash
sha256sum -c SHA256SUMS
```

> 注意: GitHubが自動生成する `Source code (zip)` および `Source code (tar.gz)` には、Kronos 5G RANのリリースパッケージは含まれていません。Release Assetsにある `kronos5gran.tar.gz` を使用してください。

### プロジェクトステータス

Kronos 5G RANは、現在主に以下の用途を想定しています。

* 評価
* 開発
* テスト
* 相互接続検証
* Proof of Concept（PoC）

今後のリリースで、各機能の動作検証および相互接続性を継続して拡張していく予定です。

### 免責事項

Kronos 5G RANは、評価、開発、テスト、PoC用途を目的とした独立実装です。

本プロジェクトは、3GPP認証取得や完全準拠を主張するものではありません。

β版として提供している機能は、完全な動作検証をまだ実施していない実験的な機能として扱ってください。

無線による送信を行う場合は、各国・地域の法令に基づく無線局免許が必要です。関係する電波法令の遵守は利用者の責任となります。
