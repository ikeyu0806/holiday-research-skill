# スキル（Claude / Codex / Cursor 共通）

**このフォルダが正本。** 手順を変えるときは**ここだけを編集する。**

各ツールの設定ファイルは、このフォルダを指す数行のポインタでしかない。ポインタ側に手順を書き足さないこと（3ツールで内容がずれる）。

## スキル一覧

| ファイル | 役割 | いつ使うか |
| --- | --- | --- |
| `tokyo-day-plan.md` | **その日の都内イベント、展覧会、公開中の映画から休日プランを作る** | 「今日何する」「東京の休日」「都内のイベント」「展覧会」「上映中の映画」「デートプラン」 |

出典URLは `references/tokyo-sources.md`。開催情報そのものはファイルに書かない。調べるたびにページを開く。

## 各ツールからの読み方

| ツール | 入口 | 発火 |
| --- | --- | --- |
| **Claude Code** | `.claude/skills/tokyo-day-plan/SKILL.md` | description で自動。`/tokyo-day-plan` でも呼べる |
| **Codex** | `AGENTS.md` と `.agents/skills/tokyo-day-plan/SKILL.md` | 共通ルールは自動。`$tokyo-day-plan` でも呼べる |
| **Cursor** | `.cursor/commands/tokyo-day-plan.md` | `/tokyo-day-plan` |
| **Cursor** | `.cursor/skills/tokyo-day-plan/SKILL.md` | description で自動 |

## 編集するとき

- 手順を変える → **このフォルダのファイルだけ**を直す
- 新しいスキルを足す → ここに `<name>.md` を作り、`.claude/skills/<name>/SKILL.md`・`.agents/skills/<name>/SKILL.md`・`.cursor/skills/<name>/SKILL.md`・`.cursor/commands/<name>.md` にポインタを足し、`AGENTS.md` とこの表に1行足す
- ポインタに手順を書かない
