# Hermes Wingtips #107: skill installs on a shared connection

posted 2026-10-20. original: [https://x.com/witcheer/status/2112446219070968105](https://x.com/witcheer/status/2112446219070968105)

the skills hub reads skills through the GitHub API, and without a token GitHub allows 60 requests an hour per network address.

one line moves your Hermes Agent onto its own budget of 5,000 an hour:

`hermes config set GITHUB_TOKEN <your token>`

docs: [https://hermes-agent.nousresearch.com/docs/user-guide/features/skills](https://hermes-agent.nousresearch.com/docs/user-guide/features/skills)
