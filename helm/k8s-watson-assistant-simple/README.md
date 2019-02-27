# Kubernetes Watson Assistant <--> Simple example
This is a slightly modified version of the Watson Assistant sample app  available with [here](https://github.com/watson-developer-cloud/assistant-simple).

This version is designed to be run on Kubernetes and includes a Helm chart that injects the required parameters as ENV vars into the container that runs the app. The values are taken from  the Helm values instead of the file **.env** that was used in the original version.

The following  values can be set  when you install the Helm Chart.

  | Name          | Description | Required ? |
  | ------------- | ----------- | ---------- |
  | assistantIamApiKey | The apikey of the Watson Assistant instance with the skill to be connected to Slack | Yes |
  | workspaceId | The Workspace ID of the Watson Assistant  skill to be connected to Slack | Yes |
  | assistantUrl | The API endpoint for the Watson Assistant instance with the skill to be connected to Slack | No |
