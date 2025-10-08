# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2025-10-08

### Added
- Initial release
- Complete category robots meta tag management
- Store view support for all attributes
- NOINDEX priority logic for products in multiple categories
- Direct SQL queries for optimal performance
- Extension point pattern integration with SeoRobotsFrontend
- Admin UI with conditional field visibility
- Support for NOARCHIVE directive
- Comprehensive documentation

### Features
- Category page robots meta tag control
- Product robots meta tag control via categories
- "Apply Robots to Products" toggle
- "Use Category Robots" option for products
- Store-specific attribute values with fallback to default
- SOLID principles compliance
- Performance-optimized SQL queries

### Technical
- Repository pattern for data access
- Service layer for business logic orchestration
- Resolver pattern for attribute value extraction
- Provider pattern for extensible robots meta tag sources
- EAV attributes for category configuration
- UI components with proper validation
