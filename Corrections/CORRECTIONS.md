# Élements de corrections

## Séance 2.

### Questions

- **Question 6.** Vous n'expliquez pas comment choisir une représentation.

- **Question 8.** Il n'existe aucune hiérarchie entre les caractères qualitatifs et les caractères quantitatifs.

### Code

- Problème d'encodage.

## Séance 3.

### Questions

- **Question 3.** Vous ne développez pas assez la moyenne.

- **Question 4.** Pas assez développée.

- **Question 5.** Il manque les déciles.

### Code

- Excellent !

- Point de détail : il aurait fallu mettre les intervalles dans le bon ordre. Cela aurait été plus facile à lire.

## Séance 4

### Questions

- Il manque beaucoup d'éléments.

### Code

- Pourquoi ne pas avoir enregistré les images comme dans les séances 2 et 3 ?

## Séance 5

### Questions

- **Question 5.** Point de détail : on parle de statistique exhaustive, et non d'enquête exhaustive, qui renvoie à la méthode de collecte.

- **Question 8.** Il manque beaucoup d'éléments.

### Code

- Pas de code pour la séance 5.

## Séance 6

### Questions

- Il manque beaucoup d'éléments.

### Code

- Beaucoup de mal à faire fonctionner votre code. Faire un P.D.F. de votre code n'était pas l'idée du siècle. À la limite, vous auriez pu m'envoyer un fichier `*.txt`.

- La fonction `def clean_numeric_series(s):` n'est pas définie. Elle est vide. Cela a pour conséquent de faire planter votre code.

    - Dans la fonction `main.py`, la variable `surfaces = clean_numeric_series(surfaces_raw)` pose problème dans l'exécution du code. De même :

```
    pop2007 = clean_numeric_series(df_monde[pop2007_col]) if pop2007_col else [float('nan')] * len(etats)
	pop2025 = clean_numeric_series(df_monde[pop2025_col]) if pop2025_col else [float('nan')] * len(etats)
	dens2007 = clean_numeric_series(df_monde[dens2007_col]) if dens2007_col else [float('nan')] * len(etats)
	dens2025 = clean_numeric_series(df_monde[dens2025_col]) if dens2025_col else [float('nan')] * len(etats)
```

    - De même, dans la fonction `def analyze_all_years_rank_concordance(df, etat_col, pop_prefix='Pop '):` avec `values = clean_numeric_series(df[colname])`.

- À quoi sert la fonction `def find_col_by_contains(possible):` ?

- Une fois ces lignes commentées et remplacées par une version sans la fonction non définie, tout fonctionne correctement.

- Le résultat concernant les tests n'est pas celui attendu.

## Humanités numériques

- Aucun rendu.

## Remarques générales

- Aucun dépôt régulier sur `GitHub`.

- Rendu n'importe que comment. Aucun temps passé à apprendre `GitHub`.

- Code non rendu dans le bon format. Comment voulez-vous que je teste un P.D.F. ?
