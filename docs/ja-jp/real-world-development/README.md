---
title: "実践的な開発"
slug: ja-jp/real-world-development
authors:
  - geektrainer
lastUpdated: 2026-09-16
---

現実的なシナリオ、完成したアプリケーション、共有バックログを使って、ソフトウェア開発ライフサイクル全体で GitHub Copilot を活用します。変更を計画し、コードを作成し、動作をテストし、pull request をレビューし、エージェントと作業を管理する流れを繰り返し実践します。

## シナリオ

架空の企業 Tailspin Toys に入社したばかりの開発者として取り組みます。同社は開発者をテーマにしたボードゲームのクラウドファンディングを運営しています。チームのバックログは GitHub issue として登録済みで、すぐに着手できます。フィルタリングやページネーションなどの機能に加え、アクセシビリティやコーディング標準に関する品質改善も含まれています。

## 作業環境を選ぶ

GitHub Copilot は、いつもの作業環境で利用できます。自分の開発スタイルに合った環境を選んでください。各ワークショップはそれぞれのセットアップから始まり、共通の Tailspin Toys シナリオを使います。

### [GitHub Copilot CLI][cli]

ターミナルでエージェント型アシスタントを使います。Plan モードと Autopilot モード、指示、スキル、カスタムエージェント、Playwright MCP、Agent Merge、実用的なスラッシュコマンドを扱います。

### [GitHub Copilot app][app]

複数のエージェントセッションを並行して実行し、セッションモードを切り替え、Canvas で共同作業し、デスクトップアプリで GitHub issue と pull request を管理します。

### [GitHub Copilot cloud agent][cloud]

GitHub issue を非同期エージェントに割り当て、作業を案内し、進行状況を監視し、エージェントが作成した pull request をレビューします。

### [Visual Studio Code][vscode]

Visual Studio Code と GitHub Codespaces で GitHub Copilot を使います。エディターを離れずに、Copilot Chat のエージェントモード、MCP サーバー、カスタムエージェントを扱います。

[cli]: cli/
[app]: app/
[cloud]: cloud/
[vscode]: vscode/
