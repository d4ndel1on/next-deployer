# next deployer

## Setup

### extend .gitignore

Add the following line to the `.gitignore`:

```
cdk.out
``` 

This makes sure that credentials are not committed to git.

### install dependencies

```bash
npm i cdk tsx
```

### deploy infrastructure
```bash
 npx -p @d4ndel1on/next-deployer next-deploy-infrastructure <env> <aws-profile>
```

### deploy frontend
```bash
 npx -p @d4ndel1on/next-deployer next-deploy <env>
```

### add github workflow [optional]

Add a github workflow to deploy the code to AWS
```bash
 npx -p @d4ndel1on/next-deployer add-workflow
```