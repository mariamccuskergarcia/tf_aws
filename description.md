# Creating a GCP function using a module

### Pre-reqs

- We will need the aws cli installed / set this up you specific 
- The trust policy and permissions policy are given in the slide deck, but can also be provided if needed.

### Scope

- Use the provided module (https://dev.azure.com/kubrick-training/ce06/_git/tf_aws_lambdafunction ) by calling it directly from the repo as a submodule to your root module to create an AWS Lambda cloud function containing the provided web scraper code.
- Structure your project with folders for `iac`, `src`
- Adhere to your naming conventions (using `locals` block)
- Use variables appropriately (don't hardcode values)
- Push code to a remote repo, include an appropriate .gitignore.- Made as repository in AzDO, have gitignore that is appropriate (ignore those terraform specific files / python venv and other commonly ignored python files)
- We will run this locally from our laptops


### Some tips:
- For this template the variable **python_source** will be `../src` (confirm that this is how you refer to a parent folder)
- When we pass a git source to a module this is the format:
```
source         = "git::https://dev.azure.com/kubrick-training/ce06/_git/tf_aws_lambdafunction"
```
