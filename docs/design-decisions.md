# Design Decisions

## 1. Group-Based Access Instead of Direct Assignments

Access was assigned through IAM-managed groups instead of assigning applications directly to users.

### Reasoning

Group-based access scales better, simplifies access reviews, reduces manual work, and supports Role-Based Access Control.

## 2. Use Existing Okta Attributes Where Available

Existing attributes such as Department, Cost Center, Manager, Organization, and Division were used instead of creating duplicates.

### Reasoning

Duplicate identity attributes create governance issues, inconsistent data, and mapping problems.

## 3. Use Enumerated Custom Attributes

Employment Type and Lifecycle Status were created as enumerated attributes.

### Reasoning

Standardized values prevent inconsistent data such as "FT", "Full Time", "fulltime", or "Employee" from breaking automation logic.

## 4. Use Okta Expression Language

Okta Expression Language was used to create multi-condition group rules.

### Reasoning

Expression Language supports more advanced logic and allows access decisions to evaluate multiple identity attributes.

## 5. Separate Lifecycle Status From Account Status

Lifecycle Status represents the business state of the user, while Okta account status controls whether the user can authenticate.

### Reasoning

A user can be marked Terminated as a business event before administrative deactivation occurs.