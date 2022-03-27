GitHubルール
===

基本的なこと
---

- ブランチ運用について
  - GitHubFlowをbaseとする
- PRについて
  - WIP PR運用だが、タイトルに```[WIP]```を記載するのではなく、ラベルで管理する。
  - 「Comment」「Request changes」を使い分けること
    - 「Comment」は、相談や提案をする。対応はレビューイに任せる。
    - 「Request changes」は修正を強制する。

プルリクエスト
---

### レビューイ/レビュイー (reviewee): レビューの依頼者

- 作業開始時
  - ブランチ作成とPR作成を行う
    - Assigneesに自分を設定する
    - Labelsを開発中的なステータスにする

- 依頼前
  - Reviewersを設定する
  - Lintをかけてから依頼を出すこと
    - LintについてのPR上の指摘は修正後「Resolve conversation（解決したよ）」を行って指摘事項を完了にしておくこと。

- レビュー後の修正
  - レビュアーからの指摘事項についてPR上ですべて返信を行うこと
    - 解決の報告をする際は、修正したコミットIDを返信すること
    - レビュアーからのコメントは「Resolve conversation（解決したよ）」を押すのはレビュアーなので押さないこと。


### レビュアー（reviewer）: レビューする人

- 初回のレビュー
  - 「Comment」「Request changes」を使い分け、レビュー結果を投稿する

- 指摘事項対応の確認
  - 修正を確認できた指摘事項は、「Resolve conversation（解決したよ）」を押す

- レビュー完了時
  - ApproveでLGTMを投稿する
  - Labelsをレビュー完了/マージ待ち的なステータスにする

### Mergeについて

- Mergeは、Squash Mergeとする
  - Merge、Rebase Mergeは禁止

