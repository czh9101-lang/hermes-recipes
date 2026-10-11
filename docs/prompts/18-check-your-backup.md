# Hermes Autopilot #18: check your latest backup would bring your setup back

posted 2026-10-11. original: [https://x.com/witcheer/status/2109229610068029620](https://x.com/witcheer/status/2109229610068029620)

this prompt gets your Hermes Agent to find your newest backup zip (the one `hermes backup` writes, [docs](https://hermes-agent.nousresearch.com/docs/reference/cli-commands#hermes-backup)), check that every file in it reads back, and open it in a temporary folder outside your Hermes home. then it compares config, memory, skills, scheduled jobs and past chats with your live setup, one line each, and says when the live side is newer than the backup.

your live setup stays as it is: nothing is restored or imported, keys and tokens are never opened, and the temporary folder is deleted only after your yes. if you have no backup yet, it asks before making one.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Check that my newest Hermes backup would bring my setup back. Look, do not change.
</role>

<principles>
<principle name="Live setup stays as it is">
Do not restore or import anything, and change nothing in my Hermes home. Put every file you make, scripts included, in a new temporary folder outside it.
</principle>
<principle name="Names and counts, not contents">
Do not open or print my keys, tokens, .env or auth files. Report file names and counts only.
</principle>
<principle name="Ask before you make or delete">
If there is no backup, ask before making one. If you cannot get my answer, end your turn and change nothing.
</principle>
</principles>

<instructions>
1. Find my newest backup zip. Tell me its name, date and size.
2. Test that every file in it reads back cleanly.
3. Unpack it into that temporary folder.
4. Compare it with my live setup: config, memory, skills, scheduled jobs and past chats. Count each side.
5. One line per item: matches, missing or a different count. Say so when the live side is newer than the backup.
6. Ask me before you delete the temporary folder. Then stop and wait for my yes.
</instructions>

<task>
Start with step one now.
</task>
```
