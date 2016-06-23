# serverless.env.yaml

The `serverless.env.yaml` file includes environment specific configuration.
Some resources might be generated by Serverless (like stage information) but you can always edit this file and add
your variables you can the reuse in the `serverless.yaml` file.

The `serverless.env.yaml` file is .gitignored by default and might contain sensitive information (such as API keys,
credentials etc.).

```yaml
vars: {}
stages:
  dev:
    vars: {}
    regions:
      aws_useast1:
        vars:
          iamRoleArnLambda: 'arn:aws:iam::12345678:role/crud-users-dev-IamRoleLambda-DJSKASD143'
```