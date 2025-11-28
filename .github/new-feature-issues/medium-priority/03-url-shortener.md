# Feature: URL Shortener Integration

## Description

Integrate a URL shortening service (short.io or similar) to create shareable short links for activities, event registrations, and certificate distributions.

## Why This Matters

- **Shareability**: Short links are easier to share via text, announcements, and QR codes
- **Tracking**: Link shorteners provide click analytics for event promotion
- **Branding**: Custom short domains can promote school branding
- **Mobile**: Shorter URLs are more mobile-friendly

## Implementation Considerations

- Integrate with short.io or similar service
- Support custom slug names (e.g., mergington.school/chess-club)
- Auto-generate slugs when custom names aren't provided
- Store mapping of short URLs to resources
- Provide analytics/click tracking display
- QR code generation for links

## Acceptance Criteria

- [ ] Admin can generate short URLs for activities
- [ ] Short URLs are customizable with slugs
- [ ] Auto-slug generation follows naming conventions
- [ ] Click analytics are tracked and displayed
- [ ] QR codes are generated for short URLs
- [ ] API integration is secure (API key management)

## Labels

`medium-priority` `feature` `admin` `integration`
