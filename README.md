# aws-ci-exp-2

First you need to create a secret with the following properties:
 - Name: `github-access-token`
 - Key: `token`
 - Value: `<GitHub-Access-Token>`


To create resources:
```
aws cloudformation deploy --stack-name="ci-exp-2" --template-file="./codebuild.yaml" --region="eu-central-1" --capabilities CAPABILITY_NAMED_IAM
```


To destroy resources:
```
aws cloudformation delete-stack --stack-name="ci-exp-2" --region="eu-central-1"
```
