# Changelog

## [1.1.1](https://github.com/NEIAAC/infra/compare/v1.1.0...v1.1.1) (2025-05-17)


### Bug Fixes

* add bugsink smtp ([fa92f3e](https://github.com/NEIAAC/infra/commit/fa92f3e5179d856c9e1ece641b6ff2d38be85893))
* remove unused dependency condition ([171f50f](https://github.com/NEIAAC/infra/commit/171f50f56eb3fdfb3991370fa4dec0785183a988))
* remove unused mysql config ([bce3bb2](https://github.com/NEIAAC/infra/commit/bce3bb21a407a007b4d136d427f8cc36e902d8ae))
* update bugsink healthcheck ([5d9053d](https://github.com/NEIAAC/infra/commit/5d9053dfb37964734cc5c09cf3d10481a470a406))
* update bugsink port mapping ([e625387](https://github.com/NEIAAC/infra/commit/e6253877b2bd7cec8d8c538284ed44e3599239fe))
* update grafana env var name ([eed3210](https://github.com/NEIAAC/infra/commit/eed32109d41f75c1ae75a14816fd48c135955d39))

## [1.1.0](https://github.com/NEIAAC/infra/compare/v1.0.1...v1.1.0) (2025-05-17)


### Features

* add sentry and uptime services ([d2c703d](https://github.com/NEIAAC/infra/commit/d2c703d7591c550ebaad1ae3612c2320c64eadf4))
* replace loki with portainer for UI management and logs ([b1de7e8](https://github.com/NEIAAC/infra/commit/b1de7e8ee589cee5db500ead8f1feff655efc528))
* simplify the stack ([01c40cd](https://github.com/NEIAAC/infra/commit/01c40cd25e85466c9db9067eabf6cabfcbf27fd6))


### Bug Fixes

* add proxy config to bugsink ([46b3ef5](https://github.com/NEIAAC/infra/commit/46b3ef563fa8b2852aa7c196b86dfbdd64dcd68b))
* remove loki dependency ([9564d7b](https://github.com/NEIAAC/infra/commit/9564d7b9e78dada6a2d2c02d51523c02a3e53e9a))
* update config ([6cbb119](https://github.com/NEIAAC/infra/commit/6cbb119d503aec6e48a255b6711b82578c01c0df))
* update portainer port ([920ac7a](https://github.com/NEIAAC/infra/commit/920ac7aba717f8b20dc19f82227b33758325242c))
* update service names ([83f93f4](https://github.com/NEIAAC/infra/commit/83f93f4eedc2f1677969d240c43b891519db112d))

## [1.0.1](https://github.com/NEIAAC/monitoring/compare/v1.0.0...v1.0.1) (2024-11-27)


### Bug Fixes

* improve label names ([cc5cfc4](https://github.com/NEIAAC/monitoring/commit/cc5cfc41a4ae9228125c29a9154e04e448653112))

## 1.0.0 (2024-11-26)


### ⚠ BREAKING CHANGES

* add loki docker logs dashboard

### Features

* add demo alert rules ([30f369d](https://github.com/NEIAAC/monitoring/commit/30f369d8a693c3f35f275f2ccc9b679ab13bf350))
* add health checks ([8362857](https://github.com/NEIAAC/monitoring/commit/8362857e4d16a2a33327253421e5d92b8c1a47a9))
* add log retention ([d3a3000](https://github.com/NEIAAC/monitoring/commit/d3a300033b5f80d433b7ef0d0571e6f2a49c0045))
* add loki docker logs dashboard ([4ca0eb1](https://github.com/NEIAAC/monitoring/commit/4ca0eb1382d733936f01eabd47226efcc5e9300f))


### Bug Fixes

* improve dash json sharing ([e8bdcc4](https://github.com/NEIAAC/monitoring/commit/e8bdcc411489523130e8faa1a43c8a9f96f06808))
* remove file mount typo ([f1bf412](https://github.com/NEIAAC/monitoring/commit/f1bf41270af0d41ae821f4969ed717b411e6bc4a))
* switch healthcheck to wget ([adee9b6](https://github.com/NEIAAC/monitoring/commit/adee9b66bf878afbb1d4bd668ac6dca4522b0e9f))
* temporarily remove broken addon ([8e33bd3](https://github.com/NEIAAC/monitoring/commit/8e33bd3b16dff520a7a0732cc55be1301799a687))
* update broken dashboard names ([432f702](https://github.com/NEIAAC/monitoring/commit/432f7025b222821da55981816043208663db7add))
* update broken datasource names in dashboards ([f5d92a0](https://github.com/NEIAAC/monitoring/commit/f5d92a09a502699f6b4b250d45d37942ea7930c0))
* update dashboard metadata ([8e14028](https://github.com/NEIAAC/monitoring/commit/8e140281ad80a0bf84389f7e1f8983de73cec26f))
* update env variable name ([c608210](https://github.com/NEIAAC/monitoring/commit/c6082101a265cd1ad8bec89ec8d278ee8a8d4689))
* update node job name in alert ([dd2bede](https://github.com/NEIAAC/monitoring/commit/dd2bedefe19b733f6870147cabad4743b818b8f1))
* update node-exporter health check ([9e67da6](https://github.com/NEIAAC/monitoring/commit/9e67da670dee78383feadd93e9b563e2fa8f97dd))
