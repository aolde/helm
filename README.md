# helm
Helm repo for charts created by @aolde

## Register repo

```
helm repo add aolde 'https://aolde.github.io/helm/'
helm repo update
helm search bredbandskollen
```

## Add new chart to repo 

```
cd charts
helm create <name>
```

## Release chart update

1. Update `Chart.yaml` `version` and `appVersion` fields.
2. Commit and push changes.
3. The github workflow will release a new chart update to the repo.