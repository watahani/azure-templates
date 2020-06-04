# Lighthouse small template

[![](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fwatahani%2Fazure-templates%2Fmaster%2Flighthouse%2FrgDelegatedResourceManagement.json)

Deploy Delegeted Resource Management.

## 事前準備

Lighthouse を有効にし、自身をサブスクリプションの所有者に設定する。

![](/assets/iam.png)

## 必要な変数

1. 委任元サブスクリプションでリソースグループの作成 (rgName)
2. 委任先テナント ID を取得 (managedByTenantId)
3. 委任先テナントに、権限割り当て用のグループを作成し Object ID を取得 (assigneeId)

![](/assets/lighthouse-deployment.png)


see more detail https://github.com/Azure/Azure-Lighthouse-samples/tree/master/templates/rg-delegated-resource-management