[![Sonar](https://github.com/PhoneTrackTeam/demo/actions/workflows/sonar.yml/badge.svg?branch=main)](https://github.com/PhoneTrackTeam/demo/actions/workflows/sonar.yml) [![Lint](https://github.com/PhoneTrackTeam/demo/actions/workflows/lint.yaml/badge.svg)](https://github.com/PhoneTrackTeam/demo/actions/workflows/lint.yaml) [![Deploy_Status](https://argocd.phonetrack.com.br/api/badge?name=audio-analysis&revision=true)](https://argocd.phonetrack.com.br/applications/audio-analysis)

<img src="http://teamcity.phonetrack.com.br/app/rest/builds/buildType:(id:Demo_Build)/statusIcon"/>

Symfony Demo Application
========================

The "Symfony Demo Application" is a reference application created to show how
to develop applications following the [Symfony Best Practices][1].

Requirements
------------

  * PHP 7.3 or higher;
  * PDO-SQLite PHP extension enabled;
  * and the [usual Symfony application requirements][2].

Installation
------------

[Download Symfony][4] to install the `symfony` binary on your computer and run
this command:

```bash
$ symfony new --demo my_project
```

Alternatively, you can use Composer:

```bash
$ composer create-project symfony/symfony-demo my_project
```

Usage
-----

There's no need to configure anything to run the application. If you have
[installed Symfony][4] binary, run this command:

```bash
$ cd my_project/
$ symfony serve
```

Then access the application in your browser at the given URL (<https://localhost:8000> by default).

If you don't have the Symfony binary installed, run `php -S localhost:8000 -t public/`
to use the built-in PHP web server or [configure a web server][3] like Nginx or
Apache to run the application.

Tests
-----

Execute this command to run tests:

```bash
$ cd my_project/
$ ./bin/phpunit
```
