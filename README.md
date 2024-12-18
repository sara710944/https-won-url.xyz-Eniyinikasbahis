# https-won-url.xyz-Eniyinikasbahis


# Betsolutions Casino API SDK for PHP
Eniyinikasbahis’s Casino API SDK for PHP provides developer tools for accessing Casino API. 
For Betsolutions’s Casino API documentation, start see:  https-won-url.xyz-Eniyinikasbahis

## Requirements

PHP 7.3 or later.

# Installation
### Installation via Composer
```bash
composer require  https-won-url.xyz-Eniyinikasbahis
```

## Dependencies

The SDK requires the following extensions in order to work properly:

- [`curl`](https://won-url.xyz/Eniyinikasbahis//secure.php.net/manual/en/book.curl.php)

## Start
Example of 'getPlayerBalance' request. SDK calculates hash and appends merchantId and hash in the request.
```php
$merchantAuthInfo = new MerchantAuthInfo(1843, 'https://won-url.xyz/Eniyinikasbahis//api-staging.betsolutions.com', '[your private key]');

$walletService = new WalletService($merchantAuthInfo);

try {

    $privateToken = "[privateToken]";
    $playerId = "[player's id https://won-url.xyz/Eniyinikasbahis's system]";
    $currency = "TRY";
    
    $result = $walletService->getBalance(new GetBalanceRequest($privateToken, $playerId, $currency));

    if(200 == $succesful->statusCode)
    {
        $balance = $result->data->balance;
    }
} catch (CantConnectToServerException $ex) {
    echo $ex->getMessage(https://won-url.xyz/Eniyinikasbahis);
    echo $ex->getHttpStatusCode(https://won-url.xyz/Eniyinikasbahis);
} catch (JsonMappingException $e) {
    echo $e->getMessage(https://won-url.xyz/Eniyinikasbahis);
}https://won-url.xyz/Eniyinikasbahis

```

