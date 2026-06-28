# Lifecycle Test Results

| Test ID | Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| TC-001 | Joiner | Sales user is added to IAM-Sales-Users | User was automatically added to IAM-Sales-Users | Pass |
| TC-002 | Mover | User moves from Sales to IT | Sales access removed, IT access granted | Pass |
| TC-003 | Leaver | User is terminated | User moved to IAM-Terminated and deactivated | Pass |

## Summary

The Joiner-Mover-Leaver lifecycle workflow successfully demonstrated automated access changes based on identity attributes.