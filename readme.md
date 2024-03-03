# AWS CloudFormation Tutorial

Tutorial for practicing CloudFormation. Create the following configurations:

<img src="./assets/img/structure.png" width=70%/>

# settings

1. Setting local Environment

    - Install AWS CLI.

      [https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/getting-started-install.html](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/getting-started-install.html)

    - Set AWS Access Key to local Environment.
      > ps> aws configure

2. Create a KeyPair named cf-tutorial-ec2-key in the AWS Management Console.

## deploy CloudFormation Template

- git clone this repository.
  > $ git clone xxxxxx

- Type Command on shell.  
  > $ aws cloudformation deploy --template-file ./cf.yaml --stack-name cf-tutorial-stg --parameter-overrides cftMyIpAddress=xxx.xxx.xxx.xxx cftEnv=Stg
  - Enter 'cftMyIpAddress', your global IP Address.
  - Enter 'cftEnv', Deploy Environment 'Dev', 'Stg' or 'Prd'.

## delete CloudFormation Stack

- Type Command on shell.
  > $ aws cloudformation delete-stack --stack-name cf-tutorial

