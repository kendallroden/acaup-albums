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

## Clone the API code 

For this sample, we will be deploying a simple front end with a backend API to Azure Container Apps using the `az containerapp up` command. Navigate to the following [repo](https://github.com/azure-samples/containerapps-albums) and select the language of your choice for the backend API. 

Upon navigating to the repo of your choice, fork the repo and retrieve the necessary command to clone to your local machine. The command should look something like the following: 

```
git clone https://github.com/$GITHUB_USERNAME/containerapps-albumapi-$LANGUAGE.git code-to-cloud
```

Replace the variables with your GitHub username and the app language you would like to use. This command will clone the code into a directory called `code-to-cloud`.

Change your directory to ensure you are pointed at the newly cloned repo 

```
cd code-to-cloud/src
```

## DELETE the dockerfile :) 

Let's experiment with one of the new capabilities of the `az containerapp up` command. Recently, support was added for deploying from repos without a dockerfile present. Let's test it out and see how it works! Delete the file called `dockerfile` from the repository.

## Deploy the Album API to Azure Container Apps 





