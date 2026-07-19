# My AI Pulse — Visual Project Tracker

Last updated: July 18, 2026, America/Chicago

## Current Position

| Workstream | Status | Evidence / Notes |
|---|---|---|
| Challenge rules verified | Done | Deadline: July 20, 2026 at 1:00 PM PT; first 100 qualifying entries |
| Existing repository audited | Done | Repository contains empty code and documentation placeholders plus one cover image |
| Product scope confirmation | Done | Noor approved the demo scope and interactive experience |
| Usable AWS account | Done | AWS access verified without exposing long-lived keys |
| Documentation | Done | README, PRD, architecture, user stories, tracker, and test plan complete |
| Application build | Done | V2 Signal Desk and three independent activity choices are working |
| AWS deployment | Done | SAM stack and public S3 application deployed in `us-east-1` |
| Autonomous Lambda proof | Done | Manual cloud invocation returned `StatusCode: 200` |
| Builder Center article | Done | Article published successfully on AWS Builder Center |
| Final submission | Done | Published July 18, 2026, ahead of the official deadline |

## Build Checklist

| Task | Category | Time Needed | Due By | Urgency | Status | Notes |
|---|---|---:|---|---|---|---|
| Verify challenge requirements | Submission | 15 min | Jul 18 | Critical | Done | Official AWS page reviewed |
| Audit GitHub repository | Repository | 15 min | Jul 18 | Critical | Done | Current code/docs placeholders are empty |
| Establish working instructions | Process | 5 min | Jul 18 | High | Done | See `AGENTS.md` |
| Obtain usable AWS account | AWS setup | 15–60 min | Jul 18 | Critical | Done | AWS access verified in CloudShell |
| Confirm MFA, region, credits, and budget | AWS safety | 15 min | Jul 18 | Critical | In Progress | Deployment region confirmed; remaining account protections should be checked after submission |
| Approve smallest qualifying MVP | Product | 10 min | Jul 18 | Critical | Done | Interactive public demo; deferred scope recorded in PRD |
| Approve AWS architecture | Architecture | 10 min | Jul 18 | Critical | Done | EventBridge → Lambda → Bedrock → S3 architecture deployed |
| Build agent and minimal output | Engineering | 90 min | Jul 18 | Critical | Done | Scheduled Signal Engine and interactive frontend built |
| Deploy and verify autonomous run | AWS | 30 min | Jul 18 | Critical | In Progress | Stack and Lambda verified; schedule and CloudWatch screenshots pending |
| Complete README and architecture docs | Documentation | 30 min | Jul 18 | High | Done | Architecture and two article diagrams created |
| Run test plan and capture evidence | Quality | 20 min | Jul 18 | Critical | In Progress | Lambda success captured; remaining AWS evidence pending |
| Draft and publish Builder Center article | Submission | 45 min | Jul 18 | Critical | Done | Article published successfully on AWS Builder Center |

## Active Blockers

| Blocker | Impact | Fastest Response | Owner |
|---|---|---|---|
| EventBridge screenshot missing | Scheduled autonomy is not yet visually proven in the article | Capture the enabled `my-ai-pulse-daily` rule | Noor + Codex |
| CloudWatch completion screenshot missing | Successful background work lacks log evidence | Capture `agent_run_completed` in the Lambda log group | Noor + Codex |
| None blocking publication | The application, article, and repository are public | Continue with evidence capture and post-challenge improvements | Noor + Codex |

## Next Gate

1. Capture the EventBridge rule and CloudWatch completion log for the project record.
2. Confirm the next scheduled pulse refresh.
3. Collect feedback before approving post-challenge product features.
