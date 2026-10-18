---
title: "レッスン 12 - GitHub Pages でサイトをデプロイする"
description: "GitHub Copilot app を使って Pages ワークフローを構成し、その pull request をレビューして、公開された Space Quiz を確認します。"
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

GitHub Pages に Space Quiz をデプロイして、誰でも試せるようにします。Copilot はワークフローを準備し、デプロイを案内できますが、変更をレビューし、サイトが公開されたことを確認するのは自分の役割です。

このレッスンでは、次のことを行います。

- Copilot に GitHub Pages のデプロイ構成を依頼します。
- マージする前に、ワークフローと pull request をレビューします。
- デプロイの状況を確認し、公開されたサイトを検証します。

## シナリオ

Space Quiz はすでに GitHub リポジトリにありますが、まだ簡単に試す方法がありません。単一ファイルのサイトを GitHub Pages で公開すれば、サーバーやランタイムの依存関係を追加せずに、公開 URL から利用できるようになります。

## Copilot にサイトのデプロイを依頼する

`space-quiz` の Copilot app セッションで、次のプロンプトを送信します。

```plaintext
このリポジトリで GitHub Pages を有効にしてください。必要であれば Web サイトをビルドして GitHub Pages にデプロイする GitHub Actions ワークフローを作成してください。README がまだない場合は、アプリとローカルでの実行方法を説明する README を追加してください。これらの変更で pull request を作成し、必須チェックに合格したらマージしてください。デプロイが成功するまで監視し、公開された Web サイトの最終 URL を報告してください。Pages の有効化やマージの権限がない場合は、何を承認または実行すればよいか具体的に伝えてください。サイトが公開されるまでは成功を報告しないでください。
```

![3 段階の図: マージ済みの space-quiz pull request、Build website・Upload artifact・Deploy to Pages の各ステップが成功した GitHub Actions のデプロイ実行、yourname.github.io/space-quiz/ で公開された Space Quiz。](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> このプロンプトは、エージェントに pull request の作成とマージ、リポジトリの Pages 設定変更を依頼します。続行する前に、差分、デプロイ権限、GitHub の承認要求を確認してください。

## ワークフローをレビューしてデプロイを確認する

1. リポジトリに README がない場合に限り、README が追加されたことを確認します。
2. ワークフローのビルドとデプロイの手順を含め、pull request の変更をレビューします。
3. 必須の pull request チェックが成功してからマージします。
4. GitHub Actions のデプロイ実行が成功するまで確認します。
5. 報告された URL を開き、Space Quiz が読み込まれることを確認します。

エージェントが Pages を有効にできない、または pull request をマージできない場合は、エージェントから示された具体的な手順に従います。デプロイが成功し、公開サイトが読み込まれるまで、作業を完了したと見なさないでください。

## まとめと次のステップ

Space Quiz を公開サイトとして利用できるようにし、エージェントの報告だけに頼らずデプロイを確認しました。続けて[レッスン 13: レビューと次のステップ][next-lesson]に進みます。

[next-lesson]: ../13-review/
