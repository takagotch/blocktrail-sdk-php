### blocktrail-sdk-php
---
https://github.com/blocktrail/blocktrail-sdk-php

```php
use Blocktrail\SDK\BlocktrailSDK;

echo "123456789 Satoshi to BTC: " . BlocktrailSDK::toBTC(12345678) . " \n";
echo "1.2345678 BTC to Satoshi: " . BlocktrailSDK::toSatoshi(1.23456789) . " \n";

require 'vendor/autoload.php';
use Blocktrail\SDK\BlocktrailSDK;
```

```sh
sudo apt-get install php5-bcmath php5-intl php5-gmp
sudo php5enmod mcrypt

extension=php_intl.dll
extension=php_gmp.dll

curl -sS https://getcomposer.org/installer | php
php composer.phar require blocktrail/blocktrail-sdk

curl.cainfo = C:\php\certs\cacert.pem

git status
TAG="v1.1.1"
TAG=$(echo $TAG | sed 's/^v//g')
sed -i 's/const SDK_VERSION= "[0-9].[0-9].[0-9]";/const SDK_VERSION = "'$TAG'";/g' src/Blocktrail.php
git commit -am "release v${TAG}"
git tag v$TAG
git push
git push --tags
```

```json
"blocktrail/blocktrail-sdk": "1.2.*"
```


