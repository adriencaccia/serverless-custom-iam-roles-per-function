# Serverless Custom Iam Roles Names Per Function

A Serverless plugin to make sure function role names are always valid, ie:

- Below the 64 characters long AWS limit
- Always unique
- Containing meaningful information

By using it, the following errors will never occur:

```
auto generated role name for function: ${functionName} is too long (over 64 chars).
Try setting a custom role name using the property: iamRoleStatementsName.
```

## Usage

Install with

```bash
yarn add --dev serverless-custom-iam-roles-per-function
```

Add `serverless-custom-iam-roles-per-function` to your serverless plugins.

## ⚠️ Dependency

This plugin depends on [`serverless-iam-roles-per-function`](https://github.com/functionalone/serverless-iam-roles-per-function)
