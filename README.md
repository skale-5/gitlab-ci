# gitlab-ci

[![pipeline status](https://git.sk5.io/thibault.ayanides/test-common-ci/badges/main/pipeline.svg)](https://git.sk5.io/thibault.ayanides/test-common-ci/-/commits/main)

[![Latest Release](https://git.sk5.io/thibault.ayanides/test-common-ci/-/badges/release.svg)](https://git.sk5.io/thibault.ayanides/test-common-ci/-/releases)

Ce repo vise à centraliser la gestion des gitlab-ci utilisées à Skale-5 (celles qui ne sont pas générées par le CICD generator)
Cela correspond par exemple aux CI utilisées en internes dans les repos cookiecutter mais aussi aux CI custom utilisées chez les clients.

## Structure

Le dossier `templates/base` contient tous des templates unitaires utilisés par le dossier `templates/worflows`.

En principe c'est les templates du dossier workflows que vous devriez utiliser.

## Exemple d'utilisations

### En utilisant un template de `workflows`

```yaml
include:
  - project: 'skale-5/gitlab-ci'
    ref: main # branch or tag to use
    file: '/templates/workflows/.gitlab-ci.terraform.yml'
```

### En utilisant un template de `base`

```yaml
stages:
- lint # stages to include

include:
  - project: 'skale-5/gitlab-ci'
    ref: main # branch or tag to use
    file: '/templates/base/.gitlab-ci.tffmt.yml'
```


## Workflow utilisant semantic-release

### Semantic-release

Il faut créer le fichier `.releaserc` dans le repo dans lequel on veut utiliser semantic-release

```json
{
  "tagFormat": "v${version}",
  "repositoryUrl": "https://git.sk5.io/XXXXXXXXXXXXXXXXXXXXXXXX",
  "plugins": [
    "@semantic-release/commit-analyzer",
    "@semantic-release/release-notes-generator",
    "@semantic-release/changelog",
    ["@semantic-release/git", {
      "assets": ["CHANGELOG.md"],
      "message": "chore(release): ${nextRelease.version}\n\n${nextRelease.notes}[skip ci]"
    }],
    "@semantic-release/gitlab"
  ],
  "branches": ["main","master"]
}
```

Un changelog est automatiquement généré