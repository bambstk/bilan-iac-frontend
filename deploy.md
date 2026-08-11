# ALED COMMENT JE VAIS FAIRE POUR DEPLOYER ????

je vais regarder un peu de doc pour commencer hihi
[ça déjà](https://learn.microsoft.com/en-us/azure/static-web-apps/static-web-apps-cli-deploy), et pour le commande cli [ici](https://learn.microsoft.com/en-us/cli/azure/staticwebapp?view=azure-cli-latest) (en y jetant un oeuil pas sur qu'elle soit utile celle là)

bon j'suis passé à coté de [ça (l'action github action)](https://github.com/Azure/static-web-apps-deploy/tree/v1)

pour connaitre le ```swa_deployment_token``` on peut utiliser cette commande ```az staticwebapp secrets list --name front-sbaivloann-bilan --query "properties.apiKey" -o tsv``` mais y a moyen de la mettre en output sur le repo terraform plus tard
et pour recuperer la clé api ``` az keyvault secret show --vault-name kv-sbaivloann-bilan-gqs --name backend-api-key --query value -o tsv``` (il faut que je m'octroie les droits si ça a été crée par le service principal)

très honnetement quasi tout le fichier à été généré par deepseek, j'ai pas le temps de tout faire, déjà je travaille sur ce brief pendant mes vacances, ça me casse les couilles, bref, on va tester.