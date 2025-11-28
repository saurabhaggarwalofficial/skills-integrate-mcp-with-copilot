# Feature: Multi-Database Support

## Description

Support separate databases for different application concerns (forms database, email database, core database) to allow for better scaling and data isolation in larger deployments.

## Why This Matters

- **Scalability**: Different databases can be scaled independently
- **Backup Strategy**: Separate databases for different concerns allows granular backup policies
- **Performance**: Isolate high-volume operations (forms, emails) from core data
- **Integration**: Easier to integrate with external systems using dedicated databases

## Implementation Considerations

- Configurable database URIs for each concern (MAIN_DB_URI, FORMS_DB_URI, MAIL_DB_URI)
- Environment-based configuration
- Connection pooling for each database
- Migrations per database
- Optional - use same database for all if not configured

## Acceptance Criteria

- [ ] Multiple database URIs can be configured via environment variables
- [ ] Application gracefully falls back to single database if not configured
- [ ] Each database has independent migrations
- [ ] Connection pooling is optimized for each database
- [ ] Documentation shows multi-database setup

## Labels

`low-priority` `feature` `infrastructure` `scalability` `optional`
