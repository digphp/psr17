# psr17

php psr17

## Installation

``` cmd
composer require digphp/psr17
```

## Usage

``` php
$factory = new \DigPHP\Psr17\Factory;

$request = $factory->createRequest(string $method, $uri);
$response = $factory->createResponse(int $code = 200, string $reasonPhrase = '');
$response = $factory->createGeneralResponse(int $code = 200, array $headers = [], string $body = null);
$server_request = $factory->createServerRequest(string $method, $uri, array $serverParams = []);
$stream = $factory->createStream(string $content = '');
$stream = $factory->createStreamFromFile(string $file, string $mode = 'r');
$stream = $factory->createStreamFromResource($resource);
$upload_file = $factory->createUploadedFile(StreamInterface $stream,int $size = null,int $error = \UPLOAD_ERR_OK,string $clientFilename = null,string $clientMediaType = null);
$uri = $factory->createUri(string $uri = '');
```
