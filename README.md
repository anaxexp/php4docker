# Docker-based PHP stack

[![Build Status](https://travis-ci.org/anaxexp/php4docker.svg?branch=master)](https://travis-ci.org/anaxexp/php4docker)

## Introduction

Docker4PHP is a set of docker images optimized for PHP. Use `docker-compose.yml` file from the [latest stable release](https://github.com/anaxexp/php4docker/releases) to spin up local environment on Linux, Mac OS X and Windows. 

* Read the docs on [**how to use**](https://docs.anaxexp.com/stacks/php/local#usage)
* Follow [us on Twitter](https://twitter.com/anaxexphq) to track future updates
* Join [community slack](https://slack.anaxexp.com) to ask questions

## Stack

The PHP stack consist of the following containers:

| Container     | Versions           | Service name    | Image                              | Default |
| ------------- | ------------------ | --------------- | ---------------------------------- | ------- |
| [Nginx]       | 1.15, 1.14, 1.13   | `nginx`         | [anaxexp/php-nginx]                  | ✓       |
| [Apache]      | 2.4                | `apache`        | [anaxexp/php-apache]                 |         |
| [PHP]         | 7.x, 5.6           | `php`           | [anaxexp/php]                        |         |
| [MariaDB]     | 10.3, 10.2, 10.1   | `mariadb`       | [anaxexp/mariadb]                    | ✓       |
| [PostgreSQL]  | 10, 9.x            | `postgres`      | [anaxexp/postgres]                   |         |
| [Redis]       | 4.0, 3.2           | `redis`         | [anaxexp/redis]                      |         |
| [Node.js]     | 9.11, 8.11, 6.14   | `node`          | [anaxexp/node]                       |         |
| [Varnish]     | 4.1                | `varnish`       | [anaxexp/varnish]                    |         |
| [Solr]        | 7.x, 6.6, 5.5      | `solr`          | [anaxexp/solr]                       |         |
| Elasticsearch | 6.x, 5.6, 5.5, 5.4 | `elasticsearch` | [anaxexp/elasticsearch]              |         |
| Kibana        | 6.x, 5.6, 5.5, 5.4 | `kibana`        | [anaxexp/kibana]                     |         |
| [Memcached]   | 1.5                | `memcached`     | [anaxexp/memcached]                  |         |
| [Webgrind]    | 1.5                | `webgrind`      | [anaxexp/webgrind]                   |         |
| [Blackfire]   | latest             | `blackfire`     | [blackfire/blackfire]              |         |
| [Rsyslog]     | latest             | `rsyslog`       | [anaxexp/rsyslog]                    |         |
| [AthenaPDF]   | 2.10.0             | `athenapdf`     | [arachnysdocker/athenapdf-service] |         |
| [Mailhog]     | latest             | `mailhog`       | [mailhog/mailhog]                  | ✓       |
| [OpenSMTPD]   | 6.0                | `opensmtpd`     | [anaxexp/opensmtpd]                  |         |
| Adminer       | 4.6                | `adminer`       | [anaxexp/adminer]                    |         |
| phpMyAdmin    | latest             | `pma`           | [phpmyadmin/phpmyadmin]            |         |
| Portainer     | latest             | `portainer`     | [portainer/portainer]              | ✓       |
| Traefik       | latest             | `traefik`       | [_/traefik]                        | ✓       |

## Documentation

Full documentation is available at https://docs.anaxexp.com/stacks/php/local

## Maintenance

We regularly update images used in this stack and release them together, see [releases page](https://github.com/anaxexp/php4docker/releases) for full changelog and update instructions.

## License

This project is licensed under the MIT open source license.

[Apache]: https://anaxexp.com/stacks/php/docs/containers/apache
[AthenaPDF]: https://anaxexp.com/stacks/php/docs/containers/athenapdf/
[Blackfire]: https://anaxexp.com/stacks/php/docs/containers/blackfire/
[Mailhog]: https://anaxexp.com/stacks/php/docs/containers/mailhog/
[MariaDB]: https://anaxexp.com/stacks/php/docs/containers/mariadb
[Memcached]: https://anaxexp.com/stacks/php/docs/containers/memcached/
[Nginx]: https://anaxexp.com/stacks/php/docs/containers/nginx
[Node.js]: https://anaxexp.com/stacks/php/docs/containers/node
[OpenSMTPD]: https://anaxexp.com/stacks/php/docs/containers/opensmtpd/
[PHP]: https://anaxexp.com/stacks/php/docs/containers/php/
[PostgreSQL]: https://anaxexp.com/stacks/php/docs/containers/postgres
[Redis]: https://anaxexp.com/stacks/php/docs/containers/redis
[Rsyslog]: https://anaxexp.com/stacks/php/docs/containers/rsyslog/
[Solr]: https://anaxexp.com/stacks/php/docs/containers/solr/
[Varnish]: https://anaxexp.com/stacks/php/docs/containers/varnish
[Webgrind]: https://anaxexp.com/stacks/php/docs/containers/webgrind/

[_/traefik]: https://hub.docker.com/_/traefik
[arachnysdocker/athenapdf-service]: https://hub.docker.com/r/arachnysdocker/athenapdf-service
[blackfire/blackfire]: https://hub.docker.com/r/blackfire/blackfire
[mailhog/mailhog]: https://hub.docker.com/r/mailhog/mailhog
[phpmyadmin/phpmyadmin]: https://hub.docker.com/r/phpmyadmin/phpmyadmin
[portainer/portainer]: https://hub.docker.com/portainer/portainer
[anaxexp/adminer]: https://hub.docker.com/r/anaxexp/adminer
[anaxexp/elasticsearch]: https://github.com/anaxexp/elasticsearch
[anaxexp/kibana]: https://github.com/anaxexp/kibana
[anaxexp/mariadb]: https://github.com/anaxexp/mariadb
[anaxexp/memcached]: https://github.com/anaxexp/memcached
[anaxexp/node]: https://github.com/anaxexp/node
[anaxexp/opensmtpd]: https://github.com/anaxexp/opensmtpd
[anaxexp/php-apache]: https://github.com/anaxexp/php-apache
[anaxexp/php-nginx]: https://github.com/anaxexp/php-nginx
[anaxexp/php]: https://github.com/anaxexp/php
[anaxexp/postgres]: https://github.com/anaxexp/postgres
[anaxexp/redis]: https://github.com/anaxexp/redis
[anaxexp/rsyslog]: https://hub.docker.com/r/anaxexp/rsyslog
[anaxexp/solr]: https://github.com/anaxexp/solr
[anaxexp/varnish]: https://github.com/anaxexp/varnish
[anaxexp/webgrind]: https://hub.docker.com/r/anaxexp/webgrind
