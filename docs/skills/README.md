# スキル（Claude / Codex / Cursor 共通）

**このフォルダが正本。** 手順を変えるときは**ここだけを編集する。**

各ツールの設定ファイルは、このフォルダを指す数行のポインタでしかない。ポインタ側に手順を書き足さないこと（3ツールで内容がずれる）。

## スキル一覧

| ファイル | 役割 | いつ使うか |
| --- | --- | --- |
| `tokyo-private-plan.md` | **仕事終わり、休日、先のプライベート予定を調べる** | 「今夜」「仕事終わり」「休日」「予約しておきたい」「舞台」「お笑い」「テレビ」「ライブ」「フェス」「スポーツ」「サウナ」「新しい施設」「展覧会」「映画」 |

出典URLは `references/tokyo-sources.md`。開催情報そのものはファイルに書かない。調べるたびにページを開く。

## 各ツールからの読み方

| ツール | 入口 | 発火 |
| --- | --- | --- |
| **Claude Code** | `.claude/skills/tokyo-private-plan/SKILL.md` | description で自動。`/tokyo-private-plan` でも呼べる |
| **Codex** | `AGENTS.md` と `.agents/skills/tokyo-private-plan/SKILL.md` | 共通ルールは自動。`$tokyo-private-plan` でも呼べる |
| **Cursor** | `.cursor/commands/tokyo-private-plan.md` | `/tokyo-private-plan` |
| **Cursor** | `.cursor/skills/tokyo-private-plan/SKILL.md` | description で自動 |

`/tokyo-day-plan` と `$tokyo-day-plan` は同じ手順への互換用入口。手順は書かず、`tokyo-private-plan.md` を指す。

## 編集するとき

- 手順を変える → **このフォルダのファイルだけ**を直す
- 新しいスキルを足す → ここに `<name>.md` を作り、`.claude/skills/<name>/SKILL.md`・`.agents/skills/<name>/SKILL.md`・`.cursor/skills/<name>/SKILL.md`・`.cursor/commands/<name>.md` にポインタを足し、`AGENTS.md` とこの表に1行足す
- ポインタに手順を書かない
