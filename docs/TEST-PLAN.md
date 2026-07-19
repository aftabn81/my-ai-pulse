# My AI Pulse — MVP Test Plan

## Test Levels

| Level | Purpose | Environment |
|---|---|---|
| Syntax | Catch invalid Python, JavaScript, and JSON | Local workspace |
| Unit/contract | Verify ranking and output rules | Local workspace |
| Infrastructure | Validate SAM template and permissions | AWS CloudShell |
| Integration | Confirm feeds, Bedrock, S3, and schedule work together | AWS |
| Experience | Confirm mobile layout and interactions | Public AWS URL |

## Acceptance Tests

| ID | Test | Expected result | Status |
|---|---|---|---|
| T-01 | Compile `backend/app.py` | No Python syntax errors | Passed |
| T-02 | Check `frontend/app.js` | No JavaScript syntax errors | Passed |
| T-03 | Parse sample `pulse.json` | Valid JSON | Passed |
| T-04 | Validate SAM template | `sam validate` succeeds | Passed |
| T-05 | Run collectors | At least three ranked candidates survive | Passed |
| T-06 | Invoke Nova Micro | Exactly three signals and three activities returned | Passed |
| T-07 | Publish pulse | S3 `data/pulse.json` has current timestamp | Passed |
| T-08 | Load public page | Page displays three signals and three activities | Passed |
| T-09 | Copy prompt | Clipboard contains exact prompt; confirmation appears | Pending deployment |
| T-10 | Complete activity | Progress becomes 100% and survives refresh | Pending deployment |
| T-11 | Share progress | Native share or clipboard fallback works | Pending deployment |
| T-12 | Verify autonomous trigger | EventBridge invocation appears in Lambda/CloudWatch evidence | Pending schedule |
| T-13 | Check mobile width | No horizontal overflow at 360 px | Pending deployment |
| T-14 | Source failure | One failed collector does not stop other collectors | Pending integration |

## Submission Evidence to Capture

- Public mobile page.
- Three live signals and three activities.
- EventBridge schedule configuration.
- Successful Lambda invocation.
- CloudWatch log showing `agent_run_completed`.
- S3 `pulse.json` generation timestamp.
- Architecture diagram.
- Public GitHub repository.
