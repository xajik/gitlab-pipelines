# Terraform 

## Save output to Env variables

TF Output will be saved to the artifact

```
  artifacts:
    paths:
      - output.json
    expire_in: 365 days
```

Save URL into your variable to use output variable in other projects: 

* `TF_STATE_OUTPUT_URL`

It will look like: 

* `https://gitlab.com/api/v4/projects/my-group%2Finfra/jobs/artifacts/main/download?job=report`

Replace `my-group` and `infra` with your group and project name.

### AWS Assume Role

Variables required for `assume_role_dotenv_template`:

* `ID_TOKEN_AUD`
* `ROLE_ARN`
* `AWS_REGION`

### Download Artifact 

Token in the environment is required to dowload the artifact woith TF output:

* `GITLAB_ACCESS_TOKEN`