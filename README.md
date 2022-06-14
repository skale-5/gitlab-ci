# gitlab-ci

Ce repo vise à centraliser la gestion des gitlab-ci utilisées à Skale-5 (celles qui ne sont pas générées par le CICD generator)
Cela correspond par exemple aux CI utilisées en internes dans les repos cookiecutter mais aussi aux CI custom utilisées chez les clients.

## Installer le gitlab-ci dans un repo existant

Ajouter le submodule

```bash
git submodule add git@git.sk5.io:skale-5/gitlab-ci.git
```

Créer un lien avec le fichier gitlab-ci voulu

```bash
ln -s gitlab-ci/gitlab-ci.XXXXX.yml .gitlab-ci.custom.yml
```


## Surcharger le gitlab-ci sans faire de modifications sur le repo

Les dossiers `custom/` sont ignorés par git et sont automatiquement inclus dans tous les templates. Il est donc possible d'y ajouter des CI spécifiques.
