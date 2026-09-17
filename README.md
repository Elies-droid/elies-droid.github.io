# elies-droid.github.io

Site de présentation personnelle d'**Elies Mlayah** : pilotage de gestion et de trésorerie
des TPE-PME (Boost Pilotage), conseil en investissement et stratégie patrimoniale
(EM Conseil Invest), vente de solutions logistiques (Certu Systems EMEA) et recherche
quantitative indépendante.

**En ligne : https://elies-droid.github.io/**

Parcours professionnel, formations et certifications avec les justificatifs consultables
en PDF, série de working papers et mémoire de recherche.

## Contenu du dépôt

| Chemin | Rôle |
| --- | --- |
| `index.html` | La page entière : HTML, CSS et JavaScript, sans dépendance ni étape de build |
| `photo.png` | Portrait |
| `banner.jpg` | Fond du bandeau d'en-tête : photographie d'Andre Benz sur Unsplash, recadrée en 1920×600 et atténuée en CSS. La source pleine résolution reste hors du dépôt. |
| `diplomas/` | Certificats en PDF liés depuis la section Education |
| `papers/` | Documents publiés, liés depuis Education et Writing. **Les sources `.docx` et les PDF y sont exclus par défaut** dans `.gitignore` ; seul le mémoire expurgé est ré-autorisé nommément |
| `404.html` | Page d'erreur |
| `robots.txt`, `sitemap.xml` | Indexation |

## Développement

Aucun outil à installer : ouvrir `index.html` dans un navigateur.
Toute modification poussée sur `main` est publiée automatiquement par GitHub Pages.

Pour ajouter un justificatif : déposer le PDF dans `diplomas/`, puis ajouter le lien sur la ligne
correspondante dans `index.html` :

```html
<span class="pdf"><a href="diplomas/mon-certificat.pdf">Certificate (PDF)</a></span>
```

### Faire avancer un papier de la section Research

Chaque papier a un statut, qui se change dans son bloc `<article class="paper">` :

1. **Brouillon** (état par défaut) : le lecteur écrit pour l'obtenir.
   ```html
   <span class="status">PDF on request</span>
   ```
2. **Publié** : déposer le PDF dans `papers/`, puis remplacer toute la ligne
   `<p class="paper-meta">` par :
   ```html
   <p class="links"><a href="papers/nom-du-papier.pdf">Read the paper (PDF)</a></p>
   ```

`papers/*.pdf` est ignoré par défaut : ajouter une exception dans `.gitignore` pour chaque
PDF destiné à la publication, après vérification qu'il ne contient ni donnée privée ni lien
vers un Drive personnel.

Pour publier un texte hors marchés : dupliquer un bloc `<article class="paper">` dans la
section `writing`.

## Contact

contact@boostpilotage.fr · [LinkedIn](https://www.linkedin.com/in/elies-mlayah-69a542246/)

---

© 2026 Elies Mlayah. Le contenu de ce site (textes, photographie, justificatifs) est protégé et
n'est pas réutilisable sans autorisation.
