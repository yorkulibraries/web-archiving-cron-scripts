## YUL Web Archiving Cron Scripts

### Description

This is a collection of shell scripts to capture, preserve, and replay York University and Government of Canada websites using [Browsertrix Crawler](https://github.com/webrecorder/browsertrix-crawler) and [pywb](https://github.com/webrecorder/pywb).

## Usage

Add to cron.

Ex:

    05 09 * * 1 bash -c 'yulWA --name "yfile" --crawl-config "/crawl-configs/yu-yfile.yaml" --crawl-dir "/browsertrix" --dedup-dir "/dedup" --import-dir "/import" --workers 8 --version 1.6.0 > /dev/null 2>&1'


### License

Public Domain

![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")
