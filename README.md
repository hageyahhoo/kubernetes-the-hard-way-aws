# kubernetes-the-hard-way-aws
This repository is for learning AWS by utilizing the original [kubernetes-the-hard-way-aws](https://github.com/prabhatsharma/kubernetes-the-hard-way-aws).
<br><br>


## How to Create A Stack via AWS CLI
1. Create a Stack
    ```
    aws cloudformation create-stack \
    --stack-name Kubernetes-The-Hard-Way \
    --template-body file://template.yaml \
    --parameters ParameterKey=KubernetesKey,ParameterValue=kubernetes
    ```
1. Check the status
    ```
    aws cloudformation describe-stacks
    ```
1. Delete the Stack
    ```
    aws cloudformation delete-stack --stack-name Kubernetes-The-Hard-Way
    ```
<br><br>


## TODO
1. Use [AWS CloudFormation](https://aws.amazon.com/jp/cloudformation/)
1. Use [AWS SAM (Serverless Application Model)](https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/what-is-sam.html)
