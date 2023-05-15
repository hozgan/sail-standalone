# SAIL STANDALONE


## Introduction

Sail provides a Docker powered local development experience for Laravel that is compatible with macOS, Windows (WSL2), and Linux. Other than Docker, no software or libraries are required to be installed on your local computer before using Sail. Sail's simple CLI means you can start building your Laravel application without any previous Docker experience.


#### Installation

```
docker run --rm \
    -v $(pwd):/opt \
    -w /opt ghcr.io/hozgan/containers:php7 \
    composer require --dev hozgan/sail-standalone --for 2.0.0 # composer version
```

**Supported PHP Versions Are:**
- PHP5 ghcr.io/hozgan/containers:php5
- PHP7 ghcr.io/hozgan/containers:php7
- PHP8 ghcr.io/hozgan/containers:php8

#### Alias

```
alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'
```

#### Initiate
```
sail init --runtime 5.6 --with mysql,redis
```
#### Sail Up / Down

Sail uses docker-compose.

```
sail up -d
```


#### Inspiration

Laravel Sail is inspired by and derived from [Vessel](https://github.com/shipping-docker/vessel) by [Chris Fidao](https://github.com/fideloper). If you're looking for a thorough introduction to Docker, check out Chris' course: [Shipping Docker](https://serversforhackers.com/shipping-docker).

## Official Documentation

Documentation for Sail can be found on the [Laravel website](https://laravel.com/docs/sail).

## Contributing

Thank you for considering contributing to Sail! You can read the contribution guide [here](.github/CONTRIBUTING.md).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

Please review [our security policy](https://github.com/laravel/sail/security/policy) on how to report security vulnerabilities.

## License

Laravel Sail is open-sourced software licensed under the [MIT license](LICENSE.md).
