## YUDL Web archiving

### Description

This is a collection of shell scripts to capture and preserve York University and Government of Canada websites using [Heritrix](https://webarchive.jira.com/wiki/display/Heritrix/Heritrix;jsessionid=B3B6591DAB2E6A92F6BBD26D8C41BE7C) with the [Web ARChive (WARC)](http://en.wikipedia.org/wiki/Web_ARChive) standard, wkhtmltopdf/image, and a descriptive metadata ([MODS](http://www.loc.gov/standards/mods/)) record.

### Requirements

* wkhtmltopdf `sudo apt-get install wkhtmltopdf`
* [wkhtmltoimage](http://code.google.com/p/wkhtmltopdf/downloads/detail?name=wkhtmltoimage-0.11.0_rc1-static-amd64.tar.bz) (put in path)
* pngcrush `sudo apt-get install pngcrush`
* [Herirtrix](https://webarchive.jira.com/wiki/display/Heritrix/Heritrix;jsessionid=B3B6591DAB2E6A92F6BBD26D8C41BE7C)

### Installation

Setup the above requirements, clone the repository, and put the shell scripts in a path that cron can execute:

    git clone https://github.com/yorkulibraries/yul-web-archiving.git
    ln -s /path/to/web/archiving/script /path/that/cron/can/execute

### Usage

Add to cron. Please use an appropriate time. Don't want to blow up anybody's server.

Ex:

    0 3 * * * bash -c '/usr/local/bin/yulWA-yfile'

### License

Public Domain

![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")

### Thanks

[Peter Binkley](http://github.com/pbinkley)
