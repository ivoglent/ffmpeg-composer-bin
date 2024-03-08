# ffmpeg-composer-bin

A simple repository for FFMPEG lib using PHP composer

*Versions:*

- ffmpeg version 6.1-static
- ffprobe version 6.1-static

## Installation

```shell
composer require --prefer-dist -vvv --profile ivoglent/ffmpeg-composer-bin
```

## Usage

Binaries of FFMPEG lib stored on @vendor/bin

```shell
vendor/bin/ffmpeg
```

and

```shell
vendor/bin/ffprobe
```

That's all

## Example usage

For use for example with [php-ffmpeg/php-ffmpeg](https://github.com/PHP-FFMpeg/PHP-FFMpeg) which support Video
manipulation and preview images on PHP.

```php
$ffmpeg = FFMpeg\FFMpeg::create(
    [
        'ffmpeg.binaries' => 'vendor/bin/ffmpeg',
        'ffprobe.binaries' => 'vendor/bin/ffprobe'
    ]
);
```
