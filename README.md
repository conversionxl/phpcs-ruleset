# CXL Coding Standards

[PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer) coding standards ruleset for the CXL projects.

## Installation

### Standalone

```
git clone https://github.com/conversionxl/phpcs-ruleset
cd phpcs-ruleset
composer install
```

### Dependency

```
composer config repositories.phpcs-ruleset vcs https://github.com/conversionxl/phpcs-ruleset
composer require cxl/phpcs-ruleset:dev-master --dev
```

Create or modify `phpcs.xml` in project root:
```xml
<?xml version="1.0"?>
<ruleset>
    <file>src</file>
    <rule ref="CXL"/>
</ruleset>
```

### Run

```
$ composer exec -v phpcs -- -s [<file>] ...
```
