#Polish Post Shipping Method

Add two shipping metchods for Polish Post:

1. Polish Post
2. Polish Post with cash on delivery

2: Install module

`composer require magento-2-polish-post-shipping-method-module`

3: Start commands

```
php bin/magento maintenance:enable
php bin/magento setup:upgrade
php bin/magento setup:di:compile
php bin/magento setup:static-content:deploy -f
php bin/magento setup:static-content:deploy pl_PL -f
php bin/magento indexer:reindex
php bin/magento cache:clean
php bin/magento cache:flush
php bin/magento maintenance:disable
chown -R www-data:www-data /var/www/outdoorzy //on nginx linux server
```