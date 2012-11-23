# York University Libraries web archiving

### Description

This is a collection of shell scripts to archive York University websites using the [Web ARChive (WARC)](http://en.wikipedia.org/wiki/Web_ARChive) in combination with the [Bagit](http://en.wikipedia.org/wiki/BagIt) spec. This is the beginnings of web archiving at YUL. 

You have to start somewhere ;)

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
