# GitHubActionsStudy
Studying is fun for me. GitHub Actions.

![FizzBuzz Continuous Integration](https://github.com/YusukeOno/GithubActionsStudy/workflows/FizzBuzz%20Continuous%20Integration/badge.svg)


## Hello, World

```
.github/workflows/hello.yml
```

## 機能について

### ワークフローとは

ワークフローとは、リポジトリー内の開発におけるなにかしらのプロセスを自動化したものです。

ワークフローは、必ずしもCI/CDだけではなく、issueやプルリクが新たに作成された時に、担当者を割り振る作業を自動化したものもワークフローのひとつです。ひとつのリポジトリーに対して、複数のワークフローを作成できます。

ワークフローは、少なくともひとつ以上の複数のジョブから構成されます。それぞれのジョブは、ワークフロー内のなにかしらのタスクを実行します。ジョブ同士は並列に実行することや、Aジョブが成功したらBジョブを実行するといった依存関係を持たせることもできます。

ジョブは、複数のステップから構成されます。ステップは、なにかしらのコマンドの実行か、なにかしらのアクションの呼び出しを行います。

アクションは、GitHubが提供する、なにかしらの処理の固まりを表す単位です。アクションは、自作することも可能ですし、コミュニティで共有されたアクションを利用することも可能です。

### ワークフローファイルの保存場所

```
.github/workflows/*.yml
```


### ワークフローの実行環境

GitHubが提供するVM（仮想マシン）と、ユーザーが構築した独自の環境（セルフホストランナー）があります。（通常は前者を利用）

#### reference link

GitHub Actionsの超基本！特別な設定が不要なCIサービス
https://qiita.com/yassun-youtube/items/72e224d9df4c0fe21f86

GitHub ActionsでLaravelのCI環境を作ってみた
https://techracho.bpsinc.jp/wingdoor/2020_07_03/93868

