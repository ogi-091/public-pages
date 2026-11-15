# public-pages

[ogi-091](https://github.com/ogi-091)が開発するアプリのプライバシーポリシーやサポートページを管理する公開リポジトリです。公開ページはGitHub Pagesで配信します。

## 公開中のプライバシーポリシー

| アプリ | 公開ページ | 本文 |
| --- | --- | --- |
| 四目並べ（Connect Four） | [プライバシーポリシー](https://ogi-091.github.io/public-pages/connect-four/privacy-policy/) | [編集対象](site/connect-four/privacy-policy/index.html) |
| 複利計算 | [プライバシーポリシー](https://ogi-091.github.io/public-pages/fukuri-keisan/privacy-policy/) | [編集対象](site/fukuri-keisan/privacy-policy/index.html) |
| Gobblet Goblins | [プライバシーポリシー](https://ogi-091.github.io/public-pages/gobblet-goblins/privacy-policy/) | [編集対象](site/gobblet-goblins/privacy-policy/index.html) |

## 共通テンプレート

- [日本語版](templates/privacy-policy.ja.md)
- [英語版](templates/privacy-policy.en.md)

テンプレートは各アプリの本文を作成するための原本です。利用者に案内する正式なポリシーは、各アプリの公開ページとします。

日英のテンプレートは同じ構成で管理します。共通条項を変更するときは、両言語の内容と対応する版番号をそろえてください。テンプレートの更新は各アプリの公開本文に自動反映されません。

## ファイル構成と公開URL

アプリごとの識別子を使って、本文を次の場所に保存します。

```text
site/<service-slug>/privacy-policy/index.html
```

公開URLは次の形式です。

```text
https://ogi-091.github.io/public-pages/<service-slug>/privacy-policy/
```

- `site/`：GitHub Pagesで配信する公開ページ
- `templates/`：公開本文を作成するための日英テンプレート。リポジトリ上では閲覧できますが、GitHub Pagesの配信対象外です。
- `.github/workflows/deploy-pages.yml`：公開ページの配信設定

## 作成・更新の手順

1. アプリの実装・SDK設定・お問い合わせフォームを確認し、扱う情報、利用目的、保存場所、送信先、保存期間、削除方法を整理します。
2. 必要な言語のテンプレートを使い、アプリ名や問い合わせ先を差し替え、該当する条項を選びます。
3. 置換箇所と作成用の注記を取り除き、アプリごとの公開HTMLに反映します。
4. 本文を実装・ストアのプライバシー申告と照合します。日英の公開版を用意する場合は、両言語で情報の取り扱いや改定日が一致していることを確認します。
5. リンクとモバイルでの表示を確認し、変更理由と対象アプリをコミットまたはプルリクエストに記録します。
6. 配信完了後に公開ページを確認し、アプリ内とストアから正しいURLにアクセスできることを確認します。

既存の公開URLは維持し、制定日・改定日とGitの変更履歴で管理します。リリース前には、情報の取り扱いに変更がないか確認してください。

## 配信

`main`ブランチの`site/**`または配信ワークフローが更新されると、GitHub Actionsが`site/`をGitHub Pagesへ配信します。手動実行にも対応しています。

READMEやテンプレートだけの更新では、公開ページの配信は実行されません。

## 公開情報の扱い

このリポジトリには公開してよい文書だけを保存します。アプリの非公開ソースコード、内部仕様、認証情報、未公開の運営者情報、実装との照合根拠は、各アプリの非公開リポジトリで管理してください。利用者向けの公開本文には、内部の確認事項や未置換のテンプレートを掲載しません。
