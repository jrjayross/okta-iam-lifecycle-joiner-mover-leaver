# Access Model

## Access Strategy

Access is granted through IAM-managed groups instead of direct user assignments.

## Groups

| Group | Criteria | Access |
|---|---|---|
| IAM-Sales-Users | Sales + Full-Time + Active | Salesforce, Slack, Zoom |
| IAM-IT-Users | IT + Full-Time + Active | Slack, Zoom |
| IAM-Contractors | Contractor + Active | Zoom |
| IAM-Terminated | Lifecycle Status = Terminated | No applications |

## Security Benefits

- Supports least privilege
- Reduces manual access assignment
- Improves onboarding consistency
- Reduces stale access after transfers
- Improves audit readiness