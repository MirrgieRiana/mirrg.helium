# mirrg.heliumポータル

## リポジトリ

- mirrg.helium.standard
  - Github https://github.com/MirrgieRiana/mirrg.helium.standard
  - Maven `https://raw.githubusercontent.com/MirrgieRiana/mirrg.helium.standard/master/maven`
- mirrg.helium.swing
  - Github https://github.com/MirrgieRiana/mirrg.helium.swing
  - Maven `https://raw.githubusercontent.com/MirrgieRiana/mirrg.helium.swing/master/maven`

## リポジトリテンプレート

- https://github.com/MirrgieRiana/mirrg.template

## 命名規則

### リポジトリ

`グループ.リポジトリグループ名.リポジトリ分野`

### プロジェクト

`グループ.リポジトリグループ名.リポジトリ分野.プロジェクトコンセプトバージョン.プロジェクト分野`

## コミットメッセージ規定

### 動作

- Aを追加した： `add: A`
- Aを削除した： `delete: A`
- Aの中のBを外に移動させた： `A.extract: B`
- Aがリポジトリ外に移動したため削除された： `drop: A`
- Aを別の更新に合わせて更新した： `update: A`
- Aを変更した： `change: A`
- Aを修正した： `fix: A`
- Aをコメントを編集した： `comment: A`
- Aをリファクタリングした： `refactor: A`
- Aの体裁を修正した： `format: A`

### 他

- AをBに追加した： `B: add: A` `B.add: A`
- AをBに変更した： `A -> B`
- CのプロパティDをAからBに変更した： `C: D: A -> B` `C.D: A -> B`
- プロジェクトA： `project{A}`
- メソッドA： `method{A}`
- ファイルA： ``` `A` ```
- AとBを追加した： `add: A, B` `add: (A, B)`
- バージョン更新： `version: 0.0.1`
- closed： `closed #1`
- 文の並列： `closed #1; add: A, B; a: (add: C, D; remove: E)`

## バージョン規定

例： `mirrg.helium.swing.nitrogen.applet` `0.0.1`
雛形： `mirrg.helium.swing.A.applet` `B.C.D`

- 設計を根本からやり直した場合、`A`を更新する。
  - 周期表でそれより1個上が存在しない元素から順番に下っていく（例：H・Cr・N）。
  - 更新後は周期表の1個下の元素になる。
- APIの破壊的変更時に`B`が変わる。
- 内部構造を大きく変えた場合に`C`が変わる。
- 小アップデートごとに`D`が変わる。
