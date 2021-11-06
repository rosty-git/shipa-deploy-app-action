# Deploy Shipa App Action

This action deploys Shipa application

## Inputs

## `file-path`

**Required** path to appDeploy.yml file.

## Example usage

```yaml
  steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Create shipa app
      uses: rostislavgit/shipa-deploy-app-action@v0.0.1
      env:
        SHIPA_TOKEN: ${{ secrets.SHIPA_TOKEN }}
        SHIPA_HOST: ${{ secrets.SHIPA_HOST }}
      with:
        file-path: './example/appDeploy.yml'
```
