# phpMyAdmin Web Server

[![CI](https://github.com/zenstruck/phpmyadmin-server/actions/workflows/ci.yml/badge.svg)](https://github.com/zenstruck/phpmyadmin-server/actions/workflows/ci.yml)
[![Latest Stable Version](http://img.shields.io/packagist/v/zenstruck/phpmyadmin-server.svg)](https://packagist.org/packages/zenstruck/phpmyadmin-server)
[![License](http://img.shields.io/packagist/l/zenstruck/phpmyadmin-server.svg)](https://packagist.org/packages/zenstruck/phpmyadmin-server)

This library gives you a `phpmyadmin` command to start/stop a php webserver running phpMyAdmin
in the background.

## Installation

### PHAR

The preferred method of installation is to use the PHAR which can be downloaded from the most
recent [Github Release](https://github.com/zenstruck/phpmyadmin-server/releases). This method
ensures you will not have any dependency conflict issue.

```bash
wget https://github.com/zenstruck/phpmyadmin-server/releases/latest/download/phpmyadmin.phar -O phpmyadmin && chmod +x phpmyadmin
mv phpmyadmin ~/bin # assumes ~/bin is in your PATH
```

### Composer

```
composer global require zenstruck/phpmyadmin-server
```

**Note**: Ensure you have `~/.composer/vendor/bin` in your `PATH` to give access to the `phpmyadmin`
command.

## Initialization

```
phpmyadmin init
```

This command will ask you questions about your setup and download the latest version of phpMyAdmin
to `~/.phpmyadmin`.

## Start/Stop Server

```
phpmyadmin
```

If you ever need to change your configuration, run `phpmyadmin init` again.
