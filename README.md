## Laravel Nova ICNDB Package
This packages uses the [ICNDB Api](http://www.icndb.com/api/) to show the random joke on a card on Laravel Nova Dashboard.

Here's how the card will look like on a dashboard.

![alt text](https://raw.githubusercontent.com/swapnilsarwe/nova-icndb/master/card.png "ICNDB Random Joke")

## Installation
You can install the packace in to a Laravel app that uses Nova via composer:
```
composer require swapnilsarwe/nova-icndb
```

As a next step you will have to register the card with your Nova App. You can achieve this by adding the package in the `cards` method of the `NovaServiceProvider`.

```php
// in app/Providers/NovaServiceProvider.php

public function cards()
{
    return [
        // ...
        new \Swapnilsarwe\NovaIcndb\NovaIcndb,
    ];
}
```

### Security

If you discover any security related issues, please email swapnilsarwe@gmail.com instead of using the issue tracker.

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.