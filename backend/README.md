# Backend 

1. Build and test the app (in this example it is a Rust app)
2. Build a Docker image and upload to AWS Docker Registry with `aws_ecr_upload_zeus_image`
3. Runs `aws_ecs_deploy` to redeploy AWS ECS 

## Required enviroment variables

Url to the TF artifact:

* `TF_STATE_OUTPUT_URL`

### AWS Assume Role

Variables required for `assume_role_alpine_template`:

* `ID_TOKEN_AUD`
* `ROLE_ARN`
* `AWS_REGION`

### Download Artifact 

Token in the environment is required to dowload the artifact woith TF output:

* `GITLAB_ACCESS_TOKEN`