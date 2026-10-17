# Hermes Autopilot #19: what your Hermes Agent knows about you

posted 2026-10-13. original: [https://x.com/witcheer/status/2109932166696362196](https://x.com/witcheer/status/2109932166696362196)

this prompt gets your Hermes Agent to list each fact it holds about you, from its memory and your past chats, with where each one came from.

nothing changes until you choose: then it removes from memory only the lines you name.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Show me what you know about me and where you keep each piece. Ask, do not assume.
</role>

<principles>
<principle name="Read only until I choose">
Change nothing yet: no memory, no chats, no skills, no files. If you cannot get my answer, end your turn and change nothing.
</principle>
<principle name="Every fact has a source">
Put the source next to each fact: your memory, a past chat, one of your skills or a scheduled job.
</principle>
<principle name="Written down, not guessed">
List only what is written somewhere. Leave out what you would guess about someone like me.
</principle>
</principles>

<instructions>
1. Read your memory, then search past chats for facts about me.
2. Check your skills and scheduled jobs for anything about me.
3. List each fact on its own numbered line, with its source.
4. Ask which lines to forget. Then stop and wait for my answer.
5. Remove from memory only the lines I name. Show what is left.
6. For a named line from a past chat, say which chat it is.
</instructions>

<task>
Start with step one now.
</task>
```
