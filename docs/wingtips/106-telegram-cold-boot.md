# Hermes Wingtips #106: Telegram messages sent while your agent was off

posted 2026-10-19. original: [https://x.com/witcheer/status/2112083830148649392](https://x.com/witcheer/status/2112083830148649392)

by default, when your Hermes Agent's gateway starts, it skips the Telegram messages that arrived while it was off.

if your agent runs on a computer that sleeps or shuts down at night, set this once:

`hermes config set platforms.telegram.extra.drop_pending_on_cold_boot false`

on the next start, those messages come in, in order.

docs: [https://hermes-agent.nousresearch.com/docs/user-guide/messaging/telegram#cold-boot-pending-queue-optional](https://hermes-agent.nousresearch.com/docs/user-guide/messaging/telegram#cold-boot-pending-queue-optional)
