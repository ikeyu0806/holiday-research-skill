# プライベートの予定を調べる

仕事終わりの夜、休日、先のプライベート予定を、都内のイベント、舞台、お笑い、テレビ、ライブ・フェス、スポーツ、サウナ、美術館・展覧会、映画、新しい施設から調べて提案するエージェントスキルです。開催情報はリポジトリに持たず、使うたびにページを開きます。

## 使い方

このリポジトリを開いた状態で、次のように頼む。

- 「今夜、仕事終わりに何する」
- 「仕事終わりに入れるサウナ」
- 「今週末、東京で見られる試合」
- 「来月までに予約しておきたいもの」
- 「今週末の舞台とお笑い」
- 「新しい都内の施設」
- `/tokyo-private-plan`（Cursor / Claude Code）
- `$tokyo-private-plan`（Codex）

`/tokyo-day-plan` と `$tokyo-day-plan` も同じ手順です。

## 構成

手順の正本は `docs/skills/tokyo-private-plan.md`。出典URLは `docs/skills/references/tokyo-sources.md`。

| ツール | 入口 |
| --- | --- |
| Claude Code | `.claude/skills/tokyo-private-plan/SKILL.md`、`CLAUDE.md` |
| Codex | `.agents/skills/tokyo-private-plan/SKILL.md`、`AGENTS.md` |
| Cursor | `.cursor/skills/tokyo-private-plan/SKILL.md`、`.cursor/commands/tokyo-private-plan.md` |

ポインタには手順を書かない。手順を変えるときは `docs/skills/` だけを編集する。
