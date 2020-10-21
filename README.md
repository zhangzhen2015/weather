<h1 align="center"> weather </h1>

<p align="center"> A weather SDK.</p>


## Installing

```shell
$ composer require zmo/weather -vvv
```

## Usage

use Zmo\Weather\Weather;

高德开放平台应用 API Key
$key = 'mock-key';
$weather = new Weather($key);

获取实时天气
$weather->getLiveWeather('天津');

获取天气预报
$weather->getForecastsWeather('天津');

获取实时天气(XML)
$weather->getWeather('天津', 'base', 'xml');

## 参数
array|string getWeather(string $city, string $type = 'base', string $format = 'json')

## Contributing

You can contribute in one of three ways:

1. File bug reports using the [issue tracker](https://github.com/zmo/weather/issues).
2. Answer questions or fix bugs on the [issue tracker](https://github.com/zmo/weather/issues).
3. Contribute new features or update the wiki.

_The code contribution process is not very formal. You just need to make sure that you follow the PSR-0, PSR-1, and PSR-2 coding guidelines. Any new code contributions must be accompanied by unit tests where applicable._

## License

MIT