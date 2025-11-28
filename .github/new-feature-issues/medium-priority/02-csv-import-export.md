# Feature: CSV Export and Import for Activity Data

## Description

Implement CSV import/export functionality to allow teachers to easily back up activity data, bulk manage participant lists, and transfer data between systems.

## Why This Matters

- **Data Management**: Teachers can organize and manage participant lists in spreadsheets
- **Backup**: Easy backup of activity and participant data
- **Bulk Operations**: Import/export for bulk edits and migrations
- **Integration**: CSV is a universal format compatible with Excel, Google Sheets, etc.

## Implementation Considerations

- Export all activities with participant lists to CSV
- Export specific activity participant lists to CSV
- Import participant lists from CSV (add to existing activity or create new)
- CSV validation and error reporting
- Headers for clarity (Activity Name, Email, Schedule, etc.)
- Support for bulk participant removal/updates

## Acceptance Criteria

- [ ] Admin can export all activities as CSV
- [ ] Admin can export specific activity participants as CSV
- [ ] Admin can import participant list from CSV
- [ ] CSV validation provides clear error messages
- [ ] CSV format is compatible with Excel/Google Sheets
- [ ] Import preview shows records before confirming
- [ ] Duplicate email detection during import

## Related Features

Pairs with:
- Persistent Database
- Admin Authentication

## Labels

`medium-priority` `feature` `admin` `data-management`
