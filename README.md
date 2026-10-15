# Martin Delville — site académique

Site Jekyll publié sur GitHub Pages : https://martin-delville.github.io/economics/

## Mettre à jour le contenu

Tout le contenu se modifie dans des fichiers texte, sans toucher au HTML :

| Quoi | Fichier |
|---|---|
| Nom, e-mail, liens (LinkedIn, Google Scholar, ORCID…), directeurs, bandeau « job market » | `_config.yml` |
| Articles (titre, co-auteurs, résumé, lien PDF/slides) | `_data/papers.yml` |
| Présentations en conférence | `_data/talks.yml` |
| Enseignement et supports de cours | `_data/teaching.yml` |
| Page CV (formation, expérience, langues…) | `_data/cv.yml` |
| Texte de présentation de la page d'accueil | `index.html` |

- Pour ajouter le PDF d'un article : déposer le fichier dans `files/papers/` puis renseigner `pdf: /files/papers/nom.pdf` dans `_data/papers.yml`.
- Pour remplacer le CV : écraser `files/Delville_CV.pdf` (garder le même nom).
- Statut d'un article : `jmp` (job market paper), `working` (working paper) ou `progress` (en cours).

## Prévisualiser en local

```
bundle install
bundle exec jekyll serve
```

puis ouvrir http://localhost:4000/economics/

Le site est déployé automatiquement par GitHub Actions à chaque push sur `master`.
