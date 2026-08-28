# jira-bolt-cron

Public GitHub Actions that pings the private [jira-bolt-automation](https://github.com/laurenbarer49/jira-bolt-automation) repo.

GitHub `schedule:` cron is delayed for hours. After each ping this workflow sleeps on the public repo (free minutes) and starts the next ping with a token, so it does not depend on cron. `schedule:` stays as a backup if a chain dies.

This repo has **no Jira credentials**. The only secret is `DISPATCH_TOKEN`.
