# Web App 

## Required enviroment variables

Url to the TF artifact:

* `TF_STATE_OUTPUT_URL`

### AWS Assume Role

Variables required for `assume_role_dotenv_template`:

* `ID_TOKEN_AUD`
* `ROLE_ARN`
* `AWS_REGION`

### Download Artifact 

Token in the environment is required to dowload the artifact woith TF output:

* `GITLAB_ACCESS_TOKEN`