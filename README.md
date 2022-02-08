# pandoc-lettre-motivation

Ceci est une template permettant de produire facilement des lettres de motivation profesionneles en français.

## Pré-requis

Il faut avoir [pandoc](https://pandoc.org/) d'installer sur la machine.

## Utilisation
Il suffit de remplacer les données du header de son fichier markdown avec les informations personnelles et du destinataire. Ensuite, on écrite sa lettre à la suite.

```markdown
---
author: Denton Robillier
datation: "Fait à Arc-sous-Mentenot, le 8 Février 2022"
objet: "Candidature au poste d'officier de santé"
from:
 - 13 rue des Flandes
 - 25270 Arc-sous-Mentenot
 - \texttt{contact@mail.com}
to: 
 - \textbf{UNICEF}
 - 3 United Nations Plaza
 - New York, New York 10017, US
signature-file: signature.png
signature-scale: 0.2
---
```

Vérifier que les fichiers cibles et que les chemins d'accès soit correct avant de lancer la commande suivante:
```bash
pandoc -d settings.yaml
```
## Exemple

[Voir le pdf d'exemple, pour une idée du rendu.](candidature-exemple.pdf)
