# Thinkphp with Adapterman

English | [中文](./thinkphp-cn.md)

```shell
# install adapterman into your project
composer require halo123450/adapterman
# start
./vendor/bin/adapterman start
```
explain:  
1.`./vendor/bin/adapterman start` Actually carried out

    /usr/bin/env php -c vendor/halo123450/adapterman/cli-php.ini vendor/halo123450/adapterman/src/start.php "$@"

2.php -c [vendor/halo123450/adapterman/cli-php.ini](https://github.com/halo123450/adapterman/blob/master/cli-php.ini) After disabling some of the built-in php functions, the adapterman framework implements these disabled functions, so that the functions under fpm will work properly under the php cli

3.[vendor/halo123450/adapterman/src/start.php](https://github.com/halo123450/adapterman/blob/master/src/start.php) The file will automatically start the server and automatically detect which framework is being used. 
among [vendor/halo123450/adapterman/src/frameworks/index.php](https://github.com/halo123450/adapterman/blob/master/src/frameworks/index.php) Detect the framework being used
View in your browser

```http://localhost:8080```
