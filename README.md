# Kaggle Actions Example

This repository provides an example of how to interact with the [Kaggle API](https://github.com/Kaggle/kaggle-api) in [GitHub actions](https://github.com/features/actions).  
The example action can be found [here](.github/workflows/kaggle_api_action_example.yml).

## Example Breakdown

The steps for accessing the Kaggle API via an action are follows:
1. Setup Python.
2. Install Kaggle Python Library via pip.
3. Execute Kaggle Commands.

## Authentication

The Kaggle API requires a username and key for authentication. To generate a token (or use an existing one), check the [Kaggle Documentation](https://www.kaggle.com/docs/api#getting-started-installation-&-authentication). Your Kaggle username and secret must be provided to the GitHub action to authenticate with the Kaggle API. This can be done through environment variables, which can be passed to the action through the use of GitHub secrets. Simply [create two secrets](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/creating-and-using-encrypted-secrets), KaggleUsername and KaggleKey, and populate them the details in your Kaggle token. 

More information on using environment variables with GitHub can be found [here](https://help.github.com/en/actions/automating-your-workflow-with-github-actions/using-environment-variables).
