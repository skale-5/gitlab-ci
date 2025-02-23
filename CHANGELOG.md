## [2.8.2](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.8.1...v2.8.2) (2025-02-23)


### Bug Fixes

* tflint docker image ([0ec3cc6](https://git.sk5.io/skale-5/gitlab-ci/commit/0ec3cc60455b939232ff5f15cce398b5b0a1c6e6))

## [2.8.1](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.8.0...v2.8.1) (2024-10-06)


### Bug Fixes

* **terraform-docs:** switch to official terraform-docs docker image ([734632c](https://git.sk5.io/skale-5/gitlab-ci/commit/734632ccec1f5e4bfad633899926a9b54a2478b4))

# [2.8.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.7.0...v2.8.0) (2023-12-03)


### Features

* **trivy:** conditionally allow failure for trivy job ([cc2dd15](https://git.sk5.io/skale-5/gitlab-ci/commit/cc2dd155bc074c5966515e28440659afa978359e))

# [2.7.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.6.2...v2.7.0) (2023-08-06)


### Features

* push helm chart to aws registry ([44773e3](https://git.sk5.io/skale-5/gitlab-ci/commit/44773e3d33c1de5416df2d995b3171f4a1625858))

## [2.6.2](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.6.1...v2.6.2) (2023-06-25)


### Bug Fixes

* do not use shallow clone with gitleaks ([c945425](https://git.sk5.io/skale-5/gitlab-ci/commit/c9454258ff1b1c0f30876eaa91d1ff4a0ea26ad0))

## [2.6.1](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.6.0...v2.6.1) (2023-06-18)


### Bug Fixes

* fix typo ([7d03183](https://git.sk5.io/skale-5/gitlab-ci/commit/7d0318333bc128d75151d8358cc5cb28a77534a3))
* **helm:** fix workflow ([c04f135](https://git.sk5.io/skale-5/gitlab-ci/commit/c04f13539c6f3a31ca2bd93c9e39350df0e502d2))

# [2.6.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.5.1...v2.6.0) (2023-06-11)


### Features

* add new workflow for helm charts ([94d0aa6](https://git.sk5.io/skale-5/gitlab-ci/commit/94d0aa61c0af87eb360c00fc27d43cdae493c0c5))

## [2.5.1](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.5.0...v2.5.1) (2023-06-04)


### Bug Fixes

* **docker-images:** add -beta to latest build ([36f922b](https://git.sk5.io/skale-5/gitlab-ci/commit/36f922b0fac77d60e5fa65da855532a25a0281f5))
* run build only on push ([8e714ff](https://git.sk5.io/skale-5/gitlab-ci/commit/8e714ff9fd919d743566c1766a4c971253b84310))

# [2.5.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.4.0...v2.5.0) (2023-05-28)


### Bug Fixes

* cant extend array, only hashes ([8edd98c](https://git.sk5.io/skale-5/gitlab-ci/commit/8edd98cbd6ebfcc0c659bc82ae075267fb2bcb33))
* CI_COMMIT_BRANCH is null when git push tag ([2fb85ac](https://git.sk5.io/skale-5/gitlab-ci/commit/2fb85ac0ef105c734e6b9a610c2bde378d376140))
* **docker-images:** fix condition on kaniko execution ([dbbe82c](https://git.sk5.io/skale-5/gitlab-ci/commit/dbbe82c3395f1b374cbc2f90d264f19dd1eeb7af))
* dont work when is first release ([a1172fc](https://git.sk5.io/skale-5/gitlab-ci/commit/a1172fcf0dbc1d14132ab1437d185ecdc6462a9c))
* fix docker image workflow ([5035b1d](https://git.sk5.io/skale-5/gitlab-ci/commit/5035b1deb78726bd47123353197c273c89bb1c58))
* fix typo ([28ae346](https://git.sk5.io/skale-5/gitlab-ci/commit/28ae346162cf5a1793b0de048b656f884ffccc9c))
* pass NEW_TAG to docker build as env var ([b28588e](https://git.sk5.io/skale-5/gitlab-ci/commit/b28588ee917d9971508bf0694a7a2408a46f2501))


### Features

* add cookiecutter-docs templates ([d72ba4a](https://git.sk5.io/skale-5/gitlab-ci/commit/d72ba4a91fe80da777fea81f5a2facf902e17996))
* add docker image ci ([e8b30ff](https://git.sk5.io/skale-5/gitlab-ci/commit/e8b30fff764cf87cca2b29885f83459f888ae3d7))
* add semantic release dryrun in all workflows ([f60d3ff](https://git.sk5.io/skale-5/gitlab-ci/commit/f60d3ffd361d799017aba78081d47a6eba8d7d24))
* **semantic-release:** add exec plugin ([65ad0fc](https://git.sk5.io/skale-5/gitlab-ci/commit/65ad0fcbc803cc9327761d525d987481e67eb0b8))
* upgrade cookiecutter-docs ([b1dc647](https://git.sk5.io/skale-5/gitlab-ci/commit/b1dc64779e5841ed9b755206ebc1d8e89d480493))
* use only one build for docker image ([d6c72ca](https://git.sk5.io/skale-5/gitlab-ci/commit/d6c72ca41cd1b29b4c3df6299d5009b5254da874))

# [2.4.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.3.0...v2.4.0) (2023-04-30)


### Features

* add semantic release to cookiecutter wf ([baf8b57](https://git.sk5.io/skale-5/gitlab-ci/commit/baf8b572a76f1f37a2bf5e1173acfdb385276291))

# [2.3.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.2.0...v2.3.0) (2023-04-23)


### Features

* add new workflows for TF-Kustomize and TF-Helm ([87c27f1](https://git.sk5.io/skale-5/gitlab-ci/commit/87c27f1ef63c9842dfc7a90a0b4a912bda042153))

# [2.2.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.1.0...v2.2.0) (2023-04-16)


### Features

* add tfmodule gitlab CI workflow ([5adca17](https://git.sk5.io/skale-5/gitlab-ci/commit/5adca1731e77ba9c4fb5629563555ac2ee7e24b0))

# [2.1.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.0.1...v2.1.0) (2023-04-09)


### Features

* add renovate ci workflow ([837482b](https://git.sk5.io/skale-5/gitlab-ci/commit/837482b720d94344c123550c8597e0728537be21))

## [2.0.1](https://git.sk5.io/skale-5/gitlab-ci/compare/v2.0.0...v2.0.1) (2023-03-26)


### Bug Fixes

* fix badges ([f37ce54](https://git.sk5.io/skale-5/gitlab-ci/commit/f37ce548e051f132ef7f92252308adfbdca416b4))

# [2.0.0](https://git.sk5.io/skale-5/gitlab-ci/compare/v1.0.0...v2.0.0) (2023-03-25)


### Features

* **semantic-release:** add basic workflow ([685a325](https://git.sk5.io/skale-5/gitlab-ci/commit/685a325fec4c84bf294a7d83a7ec8ce1106c98de))
* **semantic-release:** add scheduled workflow ([1c61a97](https://git.sk5.io/skale-5/gitlab-ci/commit/1c61a97d18ad8525edcc7b69193c2c9785ec7a55))


### BREAKING CHANGES

* **semantic-release:** rename semantic-release auto trigger workflow

# 1.0.0 (2023-03-24)


### Bug Fixes

* **cookiecutter:** fix CI ([73d8de5](https://git.sk5.io/skale-5/gitlab-ci/commit/73d8de55cb640c28910559df29e8707c7159f914))
* fix script ([c88655d](https://git.sk5.io/skale-5/gitlab-ci/commit/c88655d50d4ffceebbbda65e599d8a98a73e6c18))
* fix typo ([ef53133](https://git.sk5.io/skale-5/gitlab-ci/commit/ef53133d7f9b1f75d8ed696b3c41012cdccd376a))


### Features

* add tflint/tfsec/tffmt CI ([c9b8fe3](https://git.sk5.io/skale-5/gitlab-ci/commit/c9b8fe3567584d19fcaeaded88600717d0355a24))
* rework repo structure ([e31bd5c](https://git.sk5.io/skale-5/gitlab-ci/commit/e31bd5c956f55d032ce1b6d3458d5862e96d5117))
