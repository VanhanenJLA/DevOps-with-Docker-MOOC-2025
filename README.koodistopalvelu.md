The app containerized and deployed is a CLI program which naturally exits successful run.

However Azure Container Instance deployment reports:
Run azure/aci-deploy@v1
Deployment Succeeded.
Your App has been deployed at: http://koodistopalvelu-cli-4.swedencentral.azurecontainer.io:80/

So the app would be reachable in that URL if it were not to terminate after execution.

This is how I manually verified the execution ran successfully.

PS C:\Users\jouni\repos\VanhanenJLA\Devops-With-Docker-MOOC-2025> az container logs --resource-group rg-koodistopalvelu --name ci-koodistopalvelu-cli
Description:
  Koodistopalvelin CLI

Usage:
  Koodistopalvelu.CLI [command] [options]

Options:
  --version       Show version information
  -?, -h, --help  Show help and usage information

Commands:
  auth  The auth property
  v6    The v6 property