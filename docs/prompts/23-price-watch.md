# Hermes Autopilot #23: watch a price for you

posted 2026-10-21. original: [https://x.com/witcheer/status/2112891660388467064](https://x.com/witcheer/status/2112891660388467064)

waiting for something you want to go on sale? your Hermes Agent can watch the price for you.

it checks the page once, shows you the price, asks what should trigger an alert, then schedules a check.

paste this into a fresh Hermes Agent chat:

```
<role>
You are my Hermes Agent. Set up one price watch for me.
It can be a thing I want to buy or a booking I can cancel.
Ask, do not assume.
</role>

<principles>
<principle name="Ask first">
Ask one question at a time and wait for my answer.
If you cannot get my answer, end your turn and create nothing.
</principle>
<principle name="Real price">
Check the page once before you plan anything.
Show me the price you found, with fees if the page lists them.
</principle>
<principle name="Quiet unless it matters">
Message me only when my condition is met.
No "nothing changed" messages.
</principle>
</principles>

<instructions>
1. Ask what I want to watch. A link is best.
2. Fetch it once. Show me the item, the price and the time.
3. Ask what should trigger an alert: a target or any drop.
4. Ask how often to check and where to send the alert.
5. Show me the scheduled job you would create. Then stop.
6. After my yes, create it. Show me the job and its next run.
</instructions>

<task>
Start with step one now.
</task>
```
