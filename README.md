# @trigrun/cli

Official CLI for TrigRun.

Use `trigrun` to log in, manage jobs, inspect executions, and work with secrets and notification channels from your terminal.

## Install

```bash
npm install -g @trigrun/cli
```

## Quick Start

```bash
trigrun login -e alice@example.com -p your-secure-password
trigrun whoami
trigrun jobs list
```

## Common Commands

```bash
trigrun jobs create --name my-job --url https://example.com --kind one_time
trigrun jobs run JOB_ID
trigrun executions list --job JOB_ID
trigrun secrets create --name api-key --value "sk_live_..."
```

## Configuration

The CLI stores credentials in:

```text
~/.trigrun/config.json
```

It also supports environment variables:

```bash
export TRIGRUN_API_URL="https://api.trigrun.com"
export TRIGRUN_TOKEN="cron_pat_abc123def456..."
```

Legacy `cronctl`, `CRON_API_URL`, and `CRON_TOKEN` support remains available for compatibility.

## Docs

- CLI overview: https://docs.trigrun.com/docs/cli/overview
- CLI installation: https://docs.trigrun.com/docs/cli/installation
- CLI usage: https://docs.trigrun.com/docs/cli/usage
- Authentication: https://docs.trigrun.com/docs/getting-started/authentication
- Jobs guide: https://docs.trigrun.com/docs/guides/jobs
- Executions guide: https://docs.trigrun.com/docs/guides/executions
- Secrets guide: https://docs.trigrun.com/docs/guides/secrets
- Notifications guide: https://docs.trigrun.com/docs/guides/notifications

## More

- API base URL: `https://api.trigrun.com`
- Docs home: https://docs.trigrun.com/docs
- Issues: https://github.com/trigrun/cli/issues
