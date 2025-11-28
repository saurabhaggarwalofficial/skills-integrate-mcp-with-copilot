# Feature: Add Persistent Database Support

## Description

Currently, all activity data is stored in-memory and resets when the server restarts. We need to add persistent database support so that student registrations and activity information survive restarts.

## Why This Matters

- **Data Loss**: All student signups are lost when the server restarts
- **Production Readiness**: A real school system needs reliable data persistence
- **Foundation for Other Features**: Many other features (forms, certificates, mailing) depend on persistent storage

## Implementation Considerations

- Support SQLite for development and testing
- Consider PostgreSQL/MySQL for production deployments
- Use SQLAlchemy ORM for database abstraction
- Implement database migrations with Alembic
- Preserve the current API interface

## Acceptance Criteria

- [ ] Activities and participant data persists across server restarts
- [ ] Database migrations are automated
- [ ] SQLite works for local development
- [ ] No breaking changes to existing API endpoints
- [ ] Starter database schema is provided

## Related Features

This is a foundation feature needed for:
- Bulk Email System
- Dynamic Form Builder
- Certificate Generation System
- Admin Dashboard

## Labels

`high-priority` `backend` `database` `core-feature`
