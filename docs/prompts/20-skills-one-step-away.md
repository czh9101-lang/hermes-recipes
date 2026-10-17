# Hermes Autopilot #20: skills one step away

posted 2026-10-15. original: [https://x.com/witcheer/status/2110645602707292199](https://x.com/witcheer/status/2110645602707292199)

some of your Hermes Agent's skills need something from you before they work: a key, an app or a sign-in. this prompt gets it to check each one and list what is missing, then pick three that fit you, from its memory of you.

it only looks: it installs nothing, loads no skill and edits no settings.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Find which of your skills need something from me before they work. Ask, do not assume.
</role>

<principles>
<principle name="Nothing set up yet">
Look only: install nothing, load no skill, edit no settings. If you cannot get my answer, end your turn and write nothing.
</principle>
<principle name="Keys stay hidden">
Check only whether a key is set. Never show one, and never ask me to paste one in this chat.
</principle>
<principle name="Plain words">
For each missing piece, say what it is and where I get it, in one line I can follow without code.
</principle>
</principles>

<instructions>
1. Read the top of each skill file for what it needs: a key, a sign-in, an app or a certain computer.
2. Check this machine for each one.
3. Say how many work now, grouped by what they help with.
4. List each skill that needs one thing first, with that thing.
5. Pick the three that fit me best from your memory. Say why.
6. Draft the list as skills-to-set-up.txt and show it here. Then stop and wait for my yes.
7. After my yes, write it to this folder and tell me the path.
</instructions>

<task>
Start with step one now.
</task>
```
