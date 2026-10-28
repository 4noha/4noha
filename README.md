### Shinonome Hatsuri (東雲はつり)

Freelance engineer / VTuber. Hardware reverse engineering, embedded firmware, and tooling for AI coding agents.

- VTuber channel: https://www.youtube.com/channel/UCcG5my_y8CVvBWBZoCzwLMA
- X (Twitter): [@4noha_](https://twitter.com/4noha_)

#### macOS 上でのリバースエンジニアリング基盤

macOS には Linux の BlueZ やモニターモードに相当する低レイヤアクセスが標準で無いため、
USB 転送の観測だけから自前でスタックを組んでいる。他の BLE/Wi-Fi 機器の調査はこの上で動く。

- **[rtl8761-hci](https://github.com/4noha/rtl8761-hci)** — RTL8761 用 Pure-Python Bluetooth HCI スタック（USB 直叩き、BlueZ 不要）
- **[rtl8812bu-userspace](https://github.com/4noha/rtl8812bu-userspace)** — RTL8812BU 用 userspace Wi-Fi スタック（macOS/Linux）。ベンダーソース無し、USB 転送の観測のみから再構築。MIT

#### ハードウェア・リバースエンジニアリング

- **[diy-fido-key](https://github.com/4noha/diy-fido-key)** — ESP32-S3 で自作した USB FIDO2 セキュリティキー
- **[ddr_stamp](https://github.com/4noha/ddr_stamp)** — HX711 ロードセルを使った Bluetooth DDR コントローラ
- **[fairplay-decrypt](https://github.com/4noha/fairplay-decrypt)** — FairPlay で保護された App Store の IPA をオフライン復号（独立したキー導出）
- **[SonyNasne-debian](https://github.com/4noha/SonyNasne-debian)** — Sony nasne (CECH-ZNR2J) を解析し Debian (mipsel) を直起動させる

#### OS・システム内部

- **[openbsd-pomera-dm250](https://github.com/4noha/openbsd-pomera-dm250)** — KING JIM ポメラ DM250 に OpenBSD を載せる。カーネルパッチ・BT テザリング・suspend/resume 修正まで一式

#### AI エージェント向けツール

- **[herdr-drover](https://github.com/4noha/herdr-drover)** — AI コーディングエージェント用ターミナルマルチプレクサ「herdr」にクラウド同期を足すプラグイン
- **[drover-cloud](https://github.com/4noha/drover-cloud)** — herdr-drover を裏で支えるクラウド基盤（Cloud Run relay + Firestore）
- **[claude-master-go](https://github.com/4noha/claude-master-go)** — 複数の Claude Code セッションを集約管理するツール
- **[memvault](https://github.com/4noha/memvault)** — 共用 PC 向けの自己破壊型・一時クレデンシャル vault（単一 Go バイナリ）

#### アプリ

- **[openmoney](https://github.com/4noha/openmoney)** — 個人資産管理ツール

#### メディア・配信

- **[obs-audio-router-shm](https://github.com/4noha/obs-audio-router-shm)** — OBS Studio のオーディオソース/フィルタ（audio-router と共有メモリで連携）
- **[obs-syphon-browser](https://github.com/4noha/obs-syphon-browser)** — OBS Studio 用、Syphon サーバーをドックでプレビューするプラグイン
