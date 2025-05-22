# WHMCS + PHPStan

Static analysis for WHMCS.

- [PHPStan](https://phpstan.org/)
- [WHMCS](https://www.whmcs.com/)

## Installation

```shell
# Clone this repository

# Download latest WHMCS stubs from
# https://github.com/yeganemehr/whmcs-stub-generator/releases

# Extract stubs to stubs directory
unzip whmcs-8.8.0.zip -d stubs

# Fix "\self" in stubs
find stubs/ -type f | xargs -n 1 -- sed -i -e 's#\\self#self#'

# Install packages
composer update

# Perform static analysis
vendor/bin/phpstan
```
