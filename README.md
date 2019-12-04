# 

```bash
 
To prepare the application for deployment, use the `sam package` command. 
To deploy the application, use the `sam deploy` command. 

```
 
```bash
pip install -r requirements.txt -t ./python/
sam package  --output-template-file packaged.yaml  --s3-bucket <your_s3_bucket>
sam deploy --template-file packaged.yaml --stack-name <your_stack_name> --capabilities CAPABILITY_IAM

```
 
