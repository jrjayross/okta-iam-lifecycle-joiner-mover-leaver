# Lessons Learned

## Key Takeaways

- Identity attributes are the foundation of access automation.
- Group-based application assignments scale better than direct user assignments.
- Joiner-Mover-Leaver workflows reduce manual access errors.
- Okta Expression Language allows more flexible rule logic.
- Lifecycle testing is critical because access must change correctly during onboarding, transfers, and termination.

## Production Considerations

In a production environment, HR systems such as Workday or SAP SuccessFactors would serve as the authoritative identity source.

Lifecycle events would flow from HR into Okta, triggering downstream access changes.

Audit logs should be forwarded to a SIEM such as Microsoft Sentinel for monitoring, compliance, and investigation.

Additional controls may include:

- Manager approval workflows
- Access reviews
- Privileged access workflows
- Separation of duties checks
- SCIM provisioning to downstream applications