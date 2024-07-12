# Quicktart utilisation fichier po_role.html

Ce rapide guide permet d'executer le fichier `po_role.html`.

## Config

1. Modifier/Ajouter des entrées
   
   Le fichier contient une variable `const jsonData` ligne 98.

   Cette variable décrit les éléments affichés dans les colonnes respective et suis le schéma suivant:

```json
"Discovery": [
    {
        ...
    },
"Delivery": [...],
"Promotion": [...]

```

Pour ajouter une entrée , ajouter le block suivant dans la colonne de votre choix:

```json
{
    "name": "nom de l`élément",
    "kpis": "liste de kpi",
    "ponderation_pm": 0,
    "ponderation_po": 0
}
```

1. Modifier la ponderation

Afin d'ajuster la pondération, il faut modifier les champs `ponderation_pm` et `ponderation_po`.

Le `slider` permet de faire un +- 0,2 progressif de sur les pondérations sauf si la pondération de départ est à 0.

Une pondération de départ a 0 équivaut a une ascendance forte PO technique ou PO - PM.

## Confluence
Il est possible dans Confluence de charger une macro HTML.

1. Dans une page en mode édition, cliquez sur `Insérer des éléments -> Voir Plus`
2. Rechercher `HTML`
3. Selectionné `HTML Macro`
4. Copier le contenu du fichier `po_role.html` dans la macro

**Note**: Il se peut que la macro soit désactivé, se renseigner auprès de l'administrateur.
