# PHP HttpQuery

## Installation

Via Composer

### Add dependencies to composer
```json
    {
        "minimum-stability": "dev",
        "repositories": [
            {
                "type":"git",
                "url":"https://github.com/TsSaltan/php-http-query"
            }
        ],
        "require": {
            "tssaltan/php-http-query": "dev-master"
        }
    }
```

## Usage

### GET query
``` php
$q = new HttpQuery('https://ipinfo.io/json');
echo $q->get();
```

### POST query
``` php
$q = new HttpQuery('https://testing-post.php');
echo $q->post(['message' => 'Hello World!']);
```
