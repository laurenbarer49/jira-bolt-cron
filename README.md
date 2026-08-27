# jira-bolt-cron

Public GitHub Actions cron that pings the private [jira-bolt-automation](https://github.com/laurenbarer49/jira-bolt-automation) repo.

Private-repo `schedule:` events are delayed for hours. Public-repo cron is close enough to wall-clock that platform verdict, SM/app/web, and the board summary actually run.

This repo has **no Jira credentials**. The only secret is `DISPATCH_TOKEN`, a GitHub token that can POST `repository_dispatch` to `jira-bolt-automation`.
