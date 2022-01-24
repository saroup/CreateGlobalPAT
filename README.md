# CreateGlobalPAT

## Deploy your dev extension to Azure DevOps

Per current documentation to deploy your extension to the marketplace you should use the following command:

```shell
tfx extension publish --manifest-globs vss-extension.json --token [token]
```

The [token] here is the Azure DevOps personal access token with the Marketplace (Publish) scope and access set to **All accessible organizations**.

Note that the instructions  say to use a global PAT, but the UI doesn't allow one to select this GUID.

This small tool will help you create a global PAT that will help you publish your extension.
Be careful when using personal access tokens with broad access across the organizations you have access to.
