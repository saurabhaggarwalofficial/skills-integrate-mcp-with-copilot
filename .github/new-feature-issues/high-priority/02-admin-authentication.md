# Feature: Admin Authentication and Authorization

## Description

Teachers need a secure way to manage activities and student registrations. Currently, any user can add or remove students. We need to implement admin authentication to allow only authorized teachers to make changes.

## Why This Matters

- **Data Integrity**: Students are currently able to remove each other from activities to free up spots
- **Access Control**: Only teachers should be able to modify activity registrations
- **Feature Gate**: Needed for certificate generation, bulk email, and form creation features

## Implementation Considerations

- Implement login system for teachers
- Store credentials securely (hashed passwords)
- Use JWT or session-based authentication
- Separate student view (read-only) from admin view (full management)
- Use JSON file for teacher credentials (as per existing issue #4)

## Acceptance Criteria

- [ ] Teachers can log in with username/password
- [ ] Students see read-only view with current participants
- [ ] Only authenticated teachers can register/unregister students
- [ ] Logout functionality is available
- [ ] Session or token-based auth is implemented
- [ ] Credentials are stored securely

## Related Features

This is required for:
- Certificate generation and distribution
- Bulk email system
- Dynamic form creation
- Admin dashboard

## Labels

`high-priority` `security` `auth` `admin`
