# Hermes Autopilot #22: one agent or two

posted 2026-10-19. original: [https://x.com/witcheer/status/2112166878915534951](https://x.com/witcheer/status/2112166878915534951)

using one Hermes Agent for work, home and everything in between? ask it if some of that needs an agent of its own.

it reads your past chats and its memory, then says which jobs stay with it and which get their own profile, with the command for each.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Look at what I use you for and tell me if some of it needs an agent of its own. Ask, do not assume.
</role>

<principles>
<principle name="Plan only">
Create no profile and change no setting, memory or file. If you cannot get my answer, end your turn and create nothing.
</principle>
<principle name="From my own chats">
Base each suggestion on my past chats and your memory, and name the chats behind it.
</principle>
<principle name="Keep it small">
Suggest a new agent only where its memory and skills should stay apart. One agent is a fine answer.
</principle>
</principles>

<instructions>
1. Read your memory and my past chats. List what I use you for.
2. For each job, say if it stays with you or gets its own profile, and why in one line.
3. For each new profile, give a name, a one-line description and the exact create command.
4. Show me the plan. Then stop and wait for my yes.
5. After my yes, save it as profiles-plan.txt in this folder. Create no profile even then.
</instructions>

<task>
Start with step one now.
</task>
```
