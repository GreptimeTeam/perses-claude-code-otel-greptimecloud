# Claude Code OpenTelemetry Perses Dashboard for GreptimeCloud

![GreptimeCloud Dashboard](https://img.shields.io/badge/GreptimeCloud%20Dashboard-8322ff)

This repo hosts pre-built [Perses](https://perses.dev/) dashboards for
[Claude
Code](https://docs.anthropic.com/en/docs/claude-code/overview)'s
OpenTelemetry data, exported to
[GreptimeCloud](https://greptime.cloud) instances.

For more information, see our upcoming blog post about collecting
Claude Code usage data into GreptimeDB, using OpenTelemetry.

## Dashboard Installation

Thanks for our gitops philosophy of managing dashboards, you can
import our pre-built ones with just a few git operations.

First, clone this repo:

```
git clone https://github.com/GreptimeTeam/perses-claude-code-otel-greptimecloud.git
cd perses-claude-code-otel-greptimecloud
```

Open your GreptimeCloud instance, click workbench, and copy the
underlying git repository URL.

![Copy git url](https://github.com/user-attachments/assets/2f08c136-40d6-43cd-9119-b11b9543c836)

Add your instance's git repository URL as alternative remote in git
repo:

```
git remote add production <git-repo-url>
```

Push to your instance's git repository:

```
git push -f production main
```

Go to your GreptimeCloud instance's web UI, and refresh the page, you
get all these dashboards.
