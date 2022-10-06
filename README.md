# Container App UP with albums app

## Prereqs 

| Requirement  | Instructions |
|--|--|
| Azure account | If you don't have one, [create an account for free](https://azure.microsoft.com/free/?WT.mc_id=A261C142F). You need the *Contributor* or *Owner* permission on the Azure subscription to proceed. <br><br>Refer to [Assign Azure roles using the Azure portal](../role-based-access-control/role-assignments-portal.md?tabs=current) for details. |
| GitHub Account | Sign up for [free](https://github.com/join). |
| git | [Install git](https://git-scm.com/downloads) |
| Azure CLI | Install the [Azure CLI](/cli/azure/install-azure-cli).|


## Getting started 

### Login to Azure 
```
az login 
```

### Upgrade Azure CLI and install the latest `containerapp` cli extension 

```
az upgrade 
```
```
az extension add --name containerapp --upgrade
```

### Register the following namespaces if not already registered for your subscription
```
az provider register --namespace Microsoft.App
```
```
az provider register --namespace Microsoft.OperationalInsights
```

## 
