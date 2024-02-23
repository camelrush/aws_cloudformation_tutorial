# AWS CloudFormation Tutorial

Tutorial for practicing CloudFormation. Create the following configurations:

<img src="./assets/img/structure.png" width=70%/>

## Setting Environment

- Install AWS CLI.

  [https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/getting-started-install.html](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/getting-started-install.html)

- Set AWS Access Key to local Environment.
  > ps> aws configure

## deploy CloudFormation Template

- git clone this repository.
  > ps> git clone xxxxxx

- Type Command on Powershell.
  > ps> aws cloudformation deploy --template-file ./cf.yaml --stack-name cf-tutorial

