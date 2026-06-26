# 🔐 Terraform Azure Key Vault

This project demonstrates how to create an Azure **Key Vault** using simple Terraform code.

Azure Key Vault helps securely store and manage sensitive information such as:

* Secrets
* Passwords
* API Keys
* Certificates
* Encryption Keys

---

## 📌 Project Overview

This Terraform project creates:

✅ Azure Resource Group
✅ Azure Key Vault
✅ Access Policy for current Azure user


---

## 🏗️ Project Structure

```text
terraform-azure-key-vault/
│── main.tf
│── provider.tf
│── .gitignore
```

---

## ⚙️ Prerequisites

Before running this project, make sure you have:

* Terraform installed
* Azure Subscription
* Azure CLI installed
* Logged into Azure account

Login to Azure:

```bash
az login
```

Verify Azure account:

```bash
az account show
```

---

## 📄 Resources Used

Terraform resources used in this project:

* azurerm_resource_group
* azurerm_key_vault
* azurerm_client_config (Data Source)

---

## ▶️ Deployment Steps

Initialize Terraform:

```bash
terraform init
```

Validate Terraform code:

```bash
terraform validate
```

Preview infrastructure changes:

```bash
terraform plan
```

Deploy resources:

```bash
terraform apply -auto-approve
```

---

## 📊 Expected Output

After successful deployment:

```bash
key_vault_name = demokeyvault12345

key_vault_id = /subscriptions/xxxx/resourceGroups/demo-rg/providers/Microsoft.KeyVault/vaults/demokeyvault12345
```

---

## 🔑 Why Azure Key Vault?

Azure Key Vault provides:

✔ Secure storage of secrets
✔ Centralized credential management
✔ Access control with policies
✔ Encryption key management
✔ Better security for applications

---

## 📌 Common Use Cases

* Store database passwords
* Store API tokens
* Store certificates
* Integrate with Virtual Machines
* Integrate with Azure Kubernetes Service (AKS)
* Integrate with applications securely

---


---

## ⚠️ Important Notes

Key Vault name must be globally unique.

Example:

```hcl
name = "ranjeetkeyvault001"
```

---

## 👨‍💻 Author

Ranjeet Kumar

Terraform | Azure | DevOps Engineer

