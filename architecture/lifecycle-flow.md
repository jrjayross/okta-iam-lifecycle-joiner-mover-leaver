# Lifecycle Flow

## Joiner

1. HR creates a new user.
2. User profile attributes are populated.
3. Okta Group Rules evaluate the attributes.
4. User is automatically added to the correct IAM group.
5. Applications are assigned through group membership.

## Mover

1. User changes department.
2. Department attribute is updated.
3. Okta reevaluates group rules.
4. Old access is removed.
5. New department access is granted.

## Leaver

1. Lifecycle Status is changed to Terminated.
2. User is moved into IAM-Terminated.
3. User is deactivated.
4. Application access is removed.
5. Audit logs validate the lifecycle event.