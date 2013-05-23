# York University Libraries web archiving

### Description

This is a collection of shell scripts to archive York University and Government of Canada websites using wget with the [Web ARChive (WARC)](http://en.wikipedia.org/wiki/Web_ARChive) standard, and wkhtmltopdf/image. Each crawl is bagged using the [Bagit](http://en.wikipedia.org/wiki/BagIt) spec.

### Requirements

* wkhtmltopdf `sudo apt-get install wkhtmltopdf`
* [wkhtmltoimage](http://code.google.com/p/wkhtmltopdf/downloads/detail?name=wkhtmltoimage-0.11.0_rc1-static-amd64.tar.bz2&can=2&q=) (put in path)
* pngcrush `sudo apt-get install pngcrush`
* [wget](http://savannah.gnu.org/forum/forum.php?forum_id=7323) (>1.14)
* [bagit](https://github.com/edsu/bagit) `pip install bagit`

### Installation

Clone the repository, and put the shell scripts in a path that cron can execute

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
