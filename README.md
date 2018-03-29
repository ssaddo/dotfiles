# A propos

Ce dépôt est une bouée de sauvetage en cas de formatage et me permet de noter les choses à savoir concernant mon installation de Linux.

## Tearing Nvidia

Le pilote propriétaire nvidia rajoute un tearing atroce :

- Utiliser nvidia settings pour gérer les settings
- Exporter la configuration et ajouter  `{ ForceCompositionPipeline = On }` dans la partie metamodes de "Screen"

## Trouver le process qui utilise un port

```
sudo netstat -nlp | grep :80
