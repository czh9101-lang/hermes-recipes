# Hermes Wingtips #98: set your agent's timezone

posted 2026-10-10. original: [https://x.com/witcheer/status/2108882539788050645](https://x.com/witcheer/status/2108882539788050645)

is your Hermes Agent on a server in another timezone? give it yours:

`hermes config set timezone America/New_York`

the agent clock and your cron schedules follow that zone, so a job set for 8am runs at 8am where you are.

use your zone's IANA name, like Europe/London or Asia/Kolkata.

set it once, before your first morning brief or daily reminder!

docs: [https://hermes-agent.nousresearch.com/docs/user-guide/configuration#timezone](https://hermes-agent.nousresearch.com/docs/user-guide/configuration#timezone)
