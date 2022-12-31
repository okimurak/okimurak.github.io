+++
author = "okky"
title = "Github Project Beta に参加できたので触ってみる"
date = "2021-10-23"
tags = [
  "Github"
]
+++

こんにちは。
新しい [GitHub Project](https://github.com/features/issues) がかっこいいと思って beta に申し込んでいたのですが
先日参加ができたので、色々触ってみました。

<center><blockquote class="twitter-tweet" data-partner="tweetdeck"><p lang="ja" dir="ltr">お、Github Project Beta を試せそう！ <a href="https://t.co/wikqtnbsW3">pic.twitter.com/wikqtnbsW3</a></p>&mdash; おっきー (@okky_eng) <a href="https://twitter.com/okky_eng/status/1451182925475504148?ref_src=twsrc%5Etfw">October 21, 2021</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script></center>

## ドキュメント

以下になります。ドキュメントには無い部分も確認してみました。

[プロジェクト（ベータ）について - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/about-projects)

## View

Table と Board の 2 種類を選択できます。
Board は以前からの Project とほぼ同等です。

{{< figure src="/images/2021/1023/view-select.png" attr="View を選択" width=500 >}}

また、View はタブで管理できるため、1 つの Project に複数の View を作ることができます。

### Table View

目玉機能の 1 つとして、表形式の View が追加されました。Issue を表で管理できます。

{{< figure src="/images/2021/1023/table-view.png" width=700 >}}

{{< figure src="/images/2021/1023/add-issue-to-project.png" attr="リポジトリから Issue を検索できる" width=500 >}}

2021/10/23 現在、下記の機能を確認できました。

- 列へ Field の追加 : Issue に Field を追加できます。
- Filter : 表示されている Issue を指定した Field の条件に従ってフィルタリングできます。
- Grouping : Field の条件に従って、Issue を Grouping できます。

### Board View

旧 Project の機能に下記が追加されていました。旧 Project 同様、**Status** だけで管理する用途に見えます。

- Filter : 表示されている Issue を指定した Field の条件に従ってフィルタリングできます。

{{< figure src="/images/2021/1023/board-view.png" width=900 >}}

### 列へ Field の追加

Table の列には下記項目を追加できました。Issue に追加した Field は Project 全体で共有されます。従って、どの View でも Field を使った操作ができます。

- Title (default) : Issue の Title
- Assignees (default) : Issue に Assignee された User
- Status (default) : Issue の Status
- Label : Issue に関連付けられた Label
- Milestone : Issue に関連付けられた Milestone
- Repository : どの Repository に属するか
- [カスタムフィールド](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/creating-a-project) : 自分たちで好きなフィールドを追加できる。

#### カスタムフィールド

次の Field を追加できました。列名も編集できます。

{{< figure src="/images/2021/1023/new-field.png" attr="New Field を選択した時" width=300 >}}

##### Text

文字通り好きな Text を入れることができます。

{{< figure src="/images/2021/1023/text.png" width=300 >}}

##### Number

数字を入力できるフィールドです。

{{< figure src="/images/2021/1023/number.png" width=300 >}}

数字以外を入力すると validation が働きます。

{{< figure src="/images/2021/1023/number-validation.png" width=300 >}}

##### Date

日付を入力できるフィールドです。DatePicker もついています。

{{< figure src="/images/2021/1023/date.png" width=300 >}}

##### Single Select

単一選択ができるフィールドです。各選択要素に色をつけられなさそうなのが残念。

{{< figure src="/images/2021/1023/single-select.png" width=300 >}}

##### Iteration

[イテレーション](https://e-words.jp/w/%E3%82%A4%E3%83%86%E3%83%AC%E3%83%BC%E3%82%B7%E3%83%A7%E3%83%B3.html)を指定するためのフィールドです。

指定した期間に従ってイテレーションの項目が作成されるので、Issue に関連付けてイテレーションを管理します。

{{< figure src="/images/2021/1023/iteration.png" width=300 >}}

{{< figure src="/images/2021/1023/iteration-select.png" width=300 >}}

### Filter

表示されている Issue を指定した条件に従ってフィルタリングできます。カスタムフィールドにも対応しているようです。

{{< figure src="/images/2021/1023/filter.png" attr="Status で Filter" width=700 >}}

{{< figure src="/images/2021/1023/filter-textfield.png" attr="カスタムフィールドで Filter" width=700 >}}

なお、Board View では Status 以外の Field は見えないので、例えばカスタムフィールドで Filter すると、なぜ出てくるのかパッと見わからないですね。

(Field にどの値が設定されているかは Table View で確認する必要があります。)

{{< figure src="/images/2021/1023/board-view-filter.png" width=700 >}}

[フィルター - プロジェクト（ベータ）のビューのカスタマイズ - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/customizing-your-project-views#filter)

### Grouping

指定した条件に従って、Issue を Grouping できます。Grouping は列項目に対応します。カスタムフィールドを使ったグルーピングにも対応しているようです。

{{< figure src="/images/2021/1023/set-group.png" width=500 >}}

{{< figure src="/images/2021/1023/select-group.png" attr="どの Field で Grouping するかを選択" width=300 >}}

(※ 2021/10/23 現在 Title, Assignees, repository, label では Grouping できません。)

[グループ化 - プロジェクト（ベータ）のビューのカスタマイズ - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/customizing-your-project-views#group)

## Project Settings について

下記を設定できることを確認できました。

### Manage access

この Project を誰と閲覧、編集できるようにするのかを設定できます。

{{< figure src="/images/2021/1023/manage-access.png"width=700 >}}

### 設定した Field の編集

Fields では既に設定したカスタムフィールドと **Status** を編集できます。

{{< figure src="/images/2021/1023/edit-status.png" width=700 >}}

## コマンドパレット

「Ctrl」 + 「k」 (「Command」 + 「k」) を使ってコマンドパレットを呼び出すことができます。
コマンドパレットは Filter や Grouping など、大抵の操作はできるようです。

[プロジェクト（ベータ）のビューのカスタマイズ - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/customizing-your-project-views#command-palette)

{{< figure src="/images/2021/1023/command-palete.png" width=700 >}}

## Workflows

beta ではまだ設定できませんが、Issue のアクションによって、どのように Issue を処理するかを定義できる Workflows という機能があることを確認できました。

例えば Issue を close したときに、Issue の Field に特定の値を設定する、といったことができるみたいです。

{{< figure src="/images/2021/1023/workflows.png" attr="Condentional, Functions が気になる…" width=900 >}}

## API と Github Actions を使った自動化

API と Github Actions を使って Project の管理を自動化できます。

しっかり触れていませんが、先述した Workflows より高度な自動化は、この方法を使うんだろうと予想しています。

[プロジェクト（ベータ）の自動化 - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/automating-projects)

## まとめ

以前の Project よりもかなり使いやすくなっているように感じました。

- Table View Field や Grouping, カスタムフィールドの追加など、View の自由度が高い。
- Iteration カスタムフィールドを追加できるので、アジャイル開発にも使える。 (以前は他のプロジェクト管理ツールと Github を連携して使っていたと思っています。)
- Workflow の自動化ができること

今後も Github Project の動向に注目です。

触ってみたい方は、Github Project の Beta に参加して [プロジェクト（ベータ）のクイックスタート - GitHub Docs](https://docs.github.com/ja/issues/trying-out-the-new-projects-experience/quickstart) を参考にして試してみるとよいと思います。
