## Required Configurations

### Secrets

The following secrets are required to be set in the repository settings:

- `SCOPED_PAT`
  - This is a personal access token with the `repo` scope. This is used to checkout the repository and push any changes.
- `SALESFORCE_JWT_KEY`
  - This is the private key used to generate the JWT token. This is used to authenticate with Salesforce production.
- `SALESFORCE_JWT_SECRET_KEY`
  - This is the private key used to generate the JWT token. This is used to authenticate with Salesforce production.
- `SALESFORCE_CLIENT_ID`
  - This is the client ID used to generate the JWT token. This is used to authenticate with Salesforce production.
- `SALESFORCE_DEVHUB_USERNAME`
  - This is the username of the DevHub org. This is used to authenticate with Salesforce production.
- `SALESFORCE_TEMPLATE_CONSUMER_KEY`
  - This is the consumer key of the template org. This is used to authenticate with the template sandbox.
- `SALESFORCE_TEMPLATE_USERNAME`
  - This is the username of the template org. This is used to authenticate with the template sandbox.
- `SALESFORCE_TEMPLATE_USERNAME`
  - This is the username of the template org. This is used to authenticate with the template sandbox.
- `SALESFORCE_TEMPLATE_JWT_SECRET_KEY`
  - This is the private key used to generate the JWT token. This is used to authenticate with the template sandbox.
- `BOT_USER_EMAIL`
  - This is the email of the bot user. This is used to create pull requests against the main branch.
- `BOT_USER_NAME`
  - This is the name of the bot user. This is used to create pull requests against the main branch.
- `SANDBOX_URL_ENCRYPTION_KEY`
  - This is the key used to encrypt the sandbox URL. This is used to deploy to pull requests against the release branch to a test sandbox.

### Repository Variables

The following repository variables are required to be set in the repository settings:

- `ISSUE_BRANCH_PREFIX`
  - This is the prefix used for the issue branch. This is used to identify branches that require a sandbox.
- `RELEASE_BRANCH_PREFIX`
  - This is the prefix used for the release branch. This is used to identify branches where pull requests should be deployed to test sandbox.
- `GENERATE_RELEASE`
  - This is feature flag that is a boolean value that determines whether release notes should be generated.
- `SALESFORCE_FORMATTED_PROFILES_AND_PERMS`
  - This is a feature flag that is a boolean value that determines whether profiles and permissions should be formatted using the `profile:decompose` plugin.
