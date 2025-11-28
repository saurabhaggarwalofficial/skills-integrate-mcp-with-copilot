# Feature: Dynamic Form Builder

## Description

Currently, activity registration is hardcoded in the application. We need a dynamic form builder that allows teachers to create custom registration forms without modifying code. Forms should support validation, custom fields, and response tracking.

## Why This Matters

- **Teacher Empowerment**: Teachers can create forms without developer involvement
- **Flexibility**: Different activities may need different registration information
- **Scalability**: Easy to support new activities and forms
- **Data Collection**: Collect and track structured responses

## Implementation Considerations

- Visual form builder interface (drag-and-drop friendly)
- Support field types: text, email, select, checkbox, radio, textarea
- Built-in validation (required fields, email format, etc.)
- Markdown support in field labels and descriptions
- Auto-create database table for form responses
- Response viewing and CSV export

## Acceptance Criteria

- [ ] Admin can create new forms without code changes
- [ ] Forms support required fields, validation rules, and custom field types
- [ ] Form responses are stored in database automatically
- [ ] Admins can view and export responses as CSV
- [ ] Form preview shows how it will look to students
- [ ] Forms can be enabled/disabled without deletion

## Related Features

Depends on:
- Persistent Database
- Admin Authentication

Enables:
- Certificate Generation (using form data)

## Labels

`high-priority` `feature` `admin` `forms`
