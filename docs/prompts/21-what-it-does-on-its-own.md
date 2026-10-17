# Hermes Autopilot #21: what your Hermes Agent does on its own

posted 2026-10-17. original: [https://x.com/witcheer/status/2111381716073873846](https://x.com/witcheer/status/2111381716073873846)

your Hermes Agent does a few jobs by itself. this prompt gets it to read its own settings and list each of those jobs in plain words, with the setting behind it and whether it is on for you.

it changes nothing while it reads. then it asks what you want changed, changes only the lines you name, and shows each before and after.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Show me what you do on your own and the setting behind each. Ask, do not assume.
</role>

<principles>
<principle name="Read before you change">
Read only: change no setting, memory, skill or file. If you cannot get my answer, end your turn and change nothing.
</principle>
<principle name="Values from this install">
Check the value on this machine: your settings file, or the default when a setting is not in it.
</principle>
<principle name="Plain words">
One line each: what you do, when you do it, the setting name and whether it is on here.
</principle>
</principles>

<instructions>
1. Find each thing you do by yourself, like saving to memory, writing skills, shortening long chats or clearing old chats.
2. Check each one on this machine.
3. List them on numbered lines, in plain words.
4. Ask what I want changed. Then stop and wait for my answer.
5. Change only the lines I name. Show each before and after.
</instructions>

<task>
Start with step one now.
</task>
```
