# CXL Coding Standards

[PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) coding standards ruleset for the CXL projects.

## Installation

### Standalone

```
git clone https://github.com/conversionxl/phpcs-ruleset
cd phpcs-ruleset
composer install
```

Run with:
```
"vendor/bin/phpcs" [path] -s
```

### Dependency

```
composer require cxl/phpcs-ruleset --dev
```

Create or modify `phpcs.xml` in project root:
```xml
<?xml version="1.0"?>
<ruleset>
    <file>src</file>
    <rule ref="CXL"/>
</ruleset>
```

Run with:
```
"vendor/bin/phpcs" -s
```