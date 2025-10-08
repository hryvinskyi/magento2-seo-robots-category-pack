# Magento 2 SEO Robots Category Pack

Complete solution for managing SEO robots meta tags for categories and products in Magento 2.

## Overview

This metapackage installs all components required for category-based robots meta tag management:

- **SeoRobotsCategoryApi** - API interfaces and contracts
- **SeoRobotsCategory** - Core functionality and business logic
- **SeoRobotsCategoryAdminUi** - Admin panel UI components
- **SeoRobotsCategoryFrontend** - Frontend robots meta tag application

## Features

- **Category Robots Meta Tag** - Set robots directives for category pages
- **Apply Robots to Products** - Control whether category robots settings apply to products
- **Product Robots Meta Tag** - Set specific robots directives for products in a category
- **Store View Support** - Different robots settings per store view
- **NOINDEX Priority** - NOINDEX settings take precedence when products are in multiple categories
- **NOARCHIVE Support** - Full support for NOARCHIVE directive

## Installation

```bash
composer require hryvinskyi/magento2-seo-robots-category-pack
php bin/magento module:enable Hryvinskyi_SeoRobotsCategoryApi Hryvinskyi_SeoRobotsCategory Hryvinskyi_SeoRobotsCategoryAdminUi Hryvinskyi_SeoRobotsCategoryFrontend
php bin/magento setup:upgrade
php bin/magento cache:flush
```

## Configuration

1. Navigate to **Catalog > Categories**
2. Edit a category
3. Go to **Search Engine Optimization** section
4. Configure the following fields:
   - **Robots Meta Tag** - Robots directive for the category page
   - **Apply Robots to Category Products** - Enable to apply robots settings to products
   - **Robots for Category Products** - Robots directive for products in this category

## Available Options

- Use Config (default)
- INDEX, FOLLOW
- NOINDEX, FOLLOW
- INDEX, NOFOLLOW
- NOINDEX, NOFOLLOW
- INDEX, FOLLOW, NOARCHIVE
- NOINDEX, FOLLOW, NOARCHIVE
- INDEX, NOFOLLOW, NOARCHIVE
- NOINDEX, NOFOLLOW, NOARCHIVE
- Use Category Robots (for product robots only)

## Requirements

- PHP ^7.4|^8.0|^8.1|^8.2
- Magento 2.4.x
- hryvinskyi/magento2-seo-robots-pack

## Author

**Volodymyr Hryvinskyi**
- Email: volodymyr@hryvinskyi.com

## License

Proprietary
