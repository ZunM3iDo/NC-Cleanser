# NC-Cleanser

**NGフィルター搭載・オーバーレイ対応のコメントビューア**

## ダウンロード
   右側のReleasesからZIPファイルをダウンロードしてください

## 概要
NC-Cleanserは、配信画面やゲーム画面上にコメントを直接表示できる、透明なデスクトップオーバーレイ型コメントビューアです。
アプリ名にもなっている「Cleanser（浄化）」の通り、強力なNGフィルタリング機能を搭載しており、不快なコメントやスパムを綺麗に取り除き、快適なコメント閲覧環境を提供します。
インストール不要で１フォルダ内で完結するポータブルアプリです。

※本アプリにはコメント投稿機能はありません。
コメントの投稿はニコ生公式プレイヤーから行ってください。
ニコ生でアニメ放送を視聴することを想定して製作しています。（作者自身がそのような使い方をしたいがため）

- **強力なNGフィルター**: 単純なキーワード指定だけでなく、正規表現に対応したNGワード設定や、特定のNGユーザーの非表示機能を搭載。同じコメントを連投するユーザーを検知して自動的にNGユーザーに登録する機能付き。
- **透過オーバーレイ & 最前面表示**: 背景を透明にして常に最前面に表示できるため、ゲームや動画の邪魔にならずにコメントを流せます。
- **マウスパススルー機能**: アプリを最前面に配置したまま、背後のゲームやアプリを直接操作可能。グローバルショートカット `Ctrl+Alt+Space` でいつでも即座にクリック透過のオン/オフを切り替えられます！
- **スマートなウィンドウ収納**: 邪魔な時はワンクリックでコントロールバーだけに折りたたみ（収納）が可能。
- **高度なカスタマイズ性**: ウィンドウの位置やサイズのプリセット保存、フォント変更、背景の不透明度調整など、自分好みの環境を構築できます。

## 使い方
1. **コメントの取得開始**
   アプリ上部の接続バーに配信のURL又は番組ID(lv○○○○)を入力して接続ボタンをクリック。
   ブラウザーのアドレス欄からURLをそのままアプリ内にドラッグ＆ドロップすることもできます。
2. **NG設定・カスタマイズ**
   設定パネルを開き、お好みのフォントや透過度、そしてNGワード・NGユーザーを設定してください。
　リスト表示モード時にコメントを右クリックからNG登録することもできます。
3. **ゲーム・配信中の活用**
   最適な位置に配置したら、`Ctrl+Alt+Space` を押してマウスパススルーを有効にしてください。これでコメントを見ながら背後のアプリを操作できます。マウスパススルーを解除する時も`Ctrl+Alt+Space` です。
4. **ウィンドウサイズと位置を3つまでプリセットとして登録しておくことができます。**
   [1][2][3]ボタンをマウス左ボタン長押しでその時のウィンドウサイズと位置を登録できます。

## 開発・ビルド方法
このプロジェクトは Tauri + SvelteKit + TypeScript で構築されています。


## 利用規約（License）

本アプリは、以下の条件に従ってどなたでも自由にご利用いただけます。

### 1. 許可されること（非商用利用）
- 個人利用、趣味、教育目的での利用
- 非営利のコミュニティや活動での利用
- ご友人やSNSなどでの紹介・再配布

### 2. 禁止されること（商用利用の禁止）
- 本アプリ（またはその一部）をそのまま、あるいは改変して有償で販売すること
- 業務、会社経営、またはその他営利を目的とした環境で本アプリを利用すること
- 本アプリを利用して直接的・間接的に収益（広告収入などを含む）を得ること

### 3. 免責事項
- 本アプリの利用によって生じた、いかなる損害・不利益についても作者は一切の責任を負いません。すべて自己責任でご利用ください。



## ライセンス表記 (Third-Party Licenses)
本プロジェクト（NC-Cleanser）は、以下のオープンソースソフトウェアおよびライブラリを使用しています。各ライブラリのライセンス条項に基づき、著作権表示および許諾表示をここに掲載します。
### フロントエンド (Frontend)
* **Svelte / SvelteKit**
  * 公式サイト: [svelte.dev](https://svelte.dev/)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) svelte contributors
* **Vite**
  * 公式サイト: [vite.dev](https://vite.dev/)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) 2019-present, Yuxi (Evan) You and Vite contributors
* **TypeScript**
  * 公式サイト: [typescriptlang.org](https://www.typescriptlang.org/)
  * ライセンス: [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) Microsoft Corporation.
### バックエンド (Backend / Rust)
* **Tauri (tauri, tauri-build, tauri-plugins)**
  * 公式サイト: [tauri.app](https://tauri.app/)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) (Dual licensed)
  * 著作権: Copyright (c) 2017-present Tauri Apps team
* **Tokio**
  * 公式サイト: [tokio.rs](https://tokio.rs/)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) 2025 Tokio Contributors
* **tokio-tungstenite**
  * リポジトリ: [github.com/snapview/tokio-tungstenite](https://github.com/snapview/tokio-tungstenite)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) tokio-tungstenite Contributors
* **Serde**
  * 公式サイト: [serde.rs](https://serde.rs/)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2014 Erick Tryzelaar and David Tolnay
* **serde_json**
  * リポジトリ: [github.com/serde-rs/json](https://github.com/serde-rs/json)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2014 Erick Tryzelaar and David Tolnay
* **Regex**
  * リポジトリ: [github.com/rust-lang/regex](https://github.com/rust-lang/regex)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2014 The Rust Project Developers
* **Aho-Corasick**
  * リポジトリ: [github.com/BurntSushi/aho-corasick](https://github.com/BurntSushi/aho-corasick)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Unlicense](https://unlicense.org/)
  * 著作権: Copyright (c) 2014 Andrew Gallant
* **Reqwest**
  * リポジトリ: [github.com/seanmonstar/reqwest](https://github.com/seanmonstar/reqwest)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2016 Sean McArthur
* **prost (prost, prost-types)**
  * リポジトリ: [github.com/tokio-rs/prost](https://github.com/tokio-rs/prost)
  * ライセンス: [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2017 Dan Burkert
* **Scraper**
  * リポジトリ: [github.com/causal-agent/scraper](https://github.com/causal-agent/scraper)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) 2016 Ruud van Asseldonk
* **Bytes**
  * リポジトリ: [github.com/tokio-rs/bytes](https://github.com/tokio-rs/bytes)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT)
  * 著作権: Copyright (c) 2018 Carl Lerche
* **Anyhow**
  * リポジトリ: [github.com/dtolnay/anyhow](https://github.com/dtolnay/anyhow)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) 2019 David Tolnay
* **Notify**
  * リポジトリ: [github.com/notify-rs/notify](https://github.com/notify-rs/notify)
  * ライセンス: [CC0 1.0 Universal (Public Domain)](https://creativecommons.org/publicdomain/zero/1.0/)
  * 著作権: Copyright (c) Felix B. and contributors
* **windows-sys**
  * リポジトリ: [github.com/microsoft/windows-rs](https://github.com/microsoft/windows-rs)
  * ライセンス: [MIT License](https://opensource.org/licenses/MIT) / [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
  * 著作権: Copyright (c) Microsoft Corporation.
