# php-aliyun-open-api-cdn

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist aliyunapi/php-aliyun-open-api-cdn
```

or add

```
"aliyunapi/php-aliyun-open-api-cdn": "~1.0"
```

to the require section of your composer.json.

使用方式
------------
```
$client = new \aliyun\cdn\Client([
    'accessKeyId' => '123456',
    'accessSecret' => '123456'
]);

//@sec https://help.aliyun.com/document_detail/27158.html
$package = [
    'Action' => 'DescribeCdnService',
    //etc...
];
$response = $client->createRequest($package);
print_r($response);
exit;
```