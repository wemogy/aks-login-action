# ![wemogy](https://wemogyimages.blob.core.windows.net/logos/wemogy-github-tiny.png) AKS Login (GitHub Action)

A GitHub Action that logs in to an AKS cluster

## Usage

```yaml
- name: AKS Login
  uses: wemogy/aks-login-action
  with:
    name: my-aks-cluster
    resource-group: my-aks-resource-gropu
    client-id: ${{ secrets.AZURE_APP_ID }}
    client-secret: ${{ secrets.AZURE_PASSWORD }}
    tenant-id: ${{ secrets.AZURE_TENANT_ID }}
```

## Inputs

| Input            | Description                                  |
| ---------------- | -------------------------------------------- |
| `name`           | **Required** The name of the AKS cluster     |
| `resource-group` | **Required** The Azure Resource Group of the AKS cluster |
| `client-id` | **Required** The Azure Service Pricipal Client ID |
| `client-secret` | **Required** The Azure Service Pricipal Secret |
| `tenant-id` | **Required** The Azure Service Pricipal Tenant ID |

## Outputs

None.
