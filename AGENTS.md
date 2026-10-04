# AGENTS.md

仕事終わりの夜、休日、先のプライベート予定を、都内の催し・舞台・お笑い・テレビ・ライブ・展覧会・映画から調べるためのリポジトリです。

このファイルは、Claude Code / Codex / Cursor が共通で参照する**プロジェクト全体の指示の正本**です。エージェント固有の設定ファイルには同じ規約を複製せず、このファイルを参照させてください。手順を変えるときは、まず `docs/skills/` を更新します。

## スキル（作業手順の正本）

**手順は `docs/skills/` にあります。** Claude Code / Codex / Cursor の3つで共有しているので、手順を変えるときは `docs/skills/` だけを編集してください。

一覧: `docs/skills/README.md`

| やること | 準拠するファイル |
| --- | --- |
| **今夜、休日、先のプライベート予定。都内のイベント、舞台、お笑い、テレビ、ライブ・フェス、展覧会、映画、新しい施設、先行予約** | `docs/skills/tokyo-private-plan.md` |

「今夜」「仕事終わり」「今日何する」「明日の東京」「休日のプラン」「予約しておきたい」「舞台」「お笑い」「テレビ」「ライブ」「フェス」「新しい施設」「展覧会」「美術館」「上映中の映画」「デートでどこ行く」と言われたら、`docs/skills/tokyo-private-plan.md` を全文読んでから調べてください。Cursor / Claude Code では `/tokyo-private-plan`、Codex では `$tokyo-private-plan` でも呼べます。`/tokyo-day-plan` と `$tokyo-day-plan` は同じ手順です。

出典URLの一覧は `docs/skills/references/tokyo-sources.md`。

## 外せないルール

- **今やっている展覧会・映画・イベント・舞台・番組は、その場でページを開いて確認する。** 記憶、学習データ、このファイルの説明で開催情報や放送情報を埋めない
- **料金、休館日、開館時間、上映時刻、放送日時、予約・発売の要否は、確認できた文言だけ書く。** 確認できない項目は「未確認」とする
- **チケットの購入、予約、会員登録はしない。** ユーザーが明示したときも、このリポジトリのスキルは調査と提案まで

## 編集するとき

- 手順を変える → `docs/skills/tokyo-private-plan.md`（出典URLは `docs/skills/references/tokyo-sources.md`）
- ポインタ（`.claude/skills/`、`.cursor/skills/`、`.cursor/commands/`、`.agents/skills/`）に手順を書かない
