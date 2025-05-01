WHMCS + PHPStan

https://github.com/yeganemehr/whmcs-stub-generator/releases

```shell
unzip whmcs-8.8.0.zip -d stubs
find stubs/ -type f | xargs -n 1 -- sed -i -e 's#\\self#self#'
composer update
vendor/bin/phpstan
```
