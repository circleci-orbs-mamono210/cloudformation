[![CircleCI](https://circleci.com/gh/circleci-orbs-tm/cloudformation.svg?style=svg)](https://circleci.com/gh/circleci-orbs-tm/cloudformation)

# orbss/aws-cloudformation

Configure and install AWS CLI and manipulate aws cloudformation command in CircleCI job

## Dependencies

* [circleci/aws-cli](https://circleci.com/orbs/registry/orb/circleci/aws-cli)

## Usage

### Set up AWS Access Key

Register Access Key, Secret Access Key and default region to CircleCI Environment Variables section.

![AWS Access Key Registration](/images/aws-access-keys.png)

### Parameters and commands

See details [CircleCI Orb Registry - orbss/aws-cloudformation](https://circleci.com/orbs/registry/orb/orbss/aws-cloudformation)

### .circleci/config.yml examples

#### Checkout example

```yaml
version: 2.1

orbs:
  cloudformation: orbss/aws-cloudformation@0.1.6

workflows:
  version: 2
  stack-test:
    jobs:
      - cloudformation/create-stack:
          stack-name: my-stack
          template-file-path: cloudformation-template-file-path.yaml
          extra-arguments: --parameters ParameterKey=InstanceType,ParameterValue=t2.micro ParameterKey=KeyName,ParameterValue=circleci
      - some-jobs
      - cloudformation/delete-stack:
          requires:
            - cloudformation/create-stack
          stack-name: my-stack
```


#### Retrieve CloudFormation template file from GitHub example

```yaml
version: 2.1

orbs:
  cloudformation: orbss/aws-cloudformation@0.1.6

workflows:
  version: 2
  stack-test:
    jobs:
      - cloudformation/create-stack:
          stack-name: my-stack
          git-url: https://github.com/my-pubic-repo.git
          template-file-path: cloudformation-template-file-path.yaml
          extra-arguments: --parameters ParameterKey=InstanceType,ParameterValue=t2.micro ParameterKey=KeyName,ParameterValue=circleci
      - some-jobs
      - cloudformation/delete-stack:
          requires:
            - cloudformation/create-stack
          stack-name: my-stack
```
