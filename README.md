
## Features
Generate CF ChangeSet and send Comment to Pull Request

### **Note**
After approval, use `natluqwerty/cfn-execute-change-set@main` to deploy

## Prerequisite
Authenticate AWS Account
``` yaml
- name: Authenticate AWS
  uses: aws-actions/configure-aws-credentials@v1
  with:
    role-to-assume: arn:aws:iam::123456789100:role/my-github-actions-role
    role-session-name: DNA-Automation-Github-Actions-Session
    aws-region: ap-southeast-2
```

## Usage
```yaml
- name: Create Changesets and Send PR Comments
  uses: natluqwerty/cfn-create_changeset@main
  with:
    stack-name: your-stack-name
    template-path: path-to-the-cfn-yaml-file
    parameter-json-path: path-to-your-parameter-json-file (not mandatory)
```

## Bug Report
If you find any bug, please let `nat.lu2022@gmail.com` know !! thank you so much!!!! 😃
