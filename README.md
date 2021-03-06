# checkout-merged-branch-with-ci-info

[![GitHub last commit](https://img.shields.io/github/last-commit/suzuki-shunsuke/checkout-merged-branch-with-ci-info.svg)](https://github.com/suzuki-shunsuke/checkout-merged-branch-with-ci-info)
[![License](http://img.shields.io/badge/license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/suzuki-shunsuke/checkout-merged-branch-with-ci-info/master/LICENSE)

checkout a merged branch

## Requirement

* git
* Git repository (.git directory)
* environment variables of [ci-info](https://github.com/suzuki-shunsuke/ci-info)
  * CI_INFO_HAS_ASSOCIATED_PR
  * CI_INFO_PR_MERGED
  * CI_INFO_PR_NUMBER

## How to use

```console
$ curl -sSfL https://raw.githubusercontent.com/suzuki-shunsuke/checkout-merged-branch-with-ci-info/blob/v0.1.0-0/checkout-merged-branch | sh
```

### Usecase

Checkout a merged branch on AWS CodeBuild

```sh
eval "$(ci-info run)"
curl -sSfL https://raw.githubusercontent.com/suzuki-shunsuke/checkout-merged-branch-with-ci-info/blob/v0.1.0-0/checkout-merged-branch | sh
```

## LICENSE

[MIT](LICENSE)
