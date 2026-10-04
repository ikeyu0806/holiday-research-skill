# 東京の休日プラン

その日の都内イベント、美術館・展覧会、公開中の映画を調べて、休日の過ごし方を提案するエージェントスキルです。開催情報はリポジトリに持たず、使うたびにページを開きます。

## 使い方

このリポジトリを開いた状態で、次のように頼む。

- 「今日、東京で何する」
- 「今週末の展覧会」
- 「池袋で見られる映画」
- `/tokyo-day-plan`（Cursor / Claude Code）
- `$tokyo-day-plan`（Codex）

## 構成

手順の正本は `docs/skills/tokyo-day-plan.md`。出典URLは `docs/skills/references/tokyo-sources.md`。

| ツール | 入口 |
| --- | --- |
| Claude Code | `.claude/skills/tokyo-day-plan/SKILL.md`、`CLAUDE.md` |
| Codex | `.agents/skills/tokyo-day-plan/SKILL.md`、`AGENTS.md` |
| Cursor | `.cursor/skills/tokyo-day-plan/SKILL.md`、`.cursor/commands/tokyo-day-plan.md` |

ポインタには手順を書かない。手順を変えるときは `docs/skills/` だけを編集する。
