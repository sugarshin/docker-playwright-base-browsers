# docker-playwright-base-browsers

[![Build Status][circleci-image]][circleci-url] ![Docker Pulls](https://img.shields.io/docker/pulls/sugarshin/playwright-base-browsers?style=flat-square)

A Docker image for Playwright with a Browser pre-installed.

CircleCI example:

```yaml
jobs:
  install:
    docker:
      - image: sugarshin/playwright-base-browsers:latest
        environment:
          PLAYWRIGHT_BROWSERS_PATH: /usr/local/ms-playwright
    steps:
      - checkout
      - run: npm ci
      ...
```

[circleci-image]: https://circleci.com/gh/sugarshin/docker-playwright-base-browsers/tree/master.svg?style=svg&circle-token=ad85a9656428647fa2e772c8622f6ff4a511065c
[circleci-url]: https://circleci.com/gh/sugarshin/docker-playwright-base-browsers/tree/master
