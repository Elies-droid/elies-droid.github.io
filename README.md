# elies-droid.github.io

Site de présentation personnelle d'**Elies Mlayah** : recherche quantitative sur futures
indiciels CME (MHE Capital) et conseil en investissement et stratégie patrimoniale
(EM Conseil Invest).

**En ligne : https://elies-droid.github.io/**

Série de working papers, parcours professionnel, formations et certifications avec les
justificatifs consultables en PDF.

## Contenu du dépôt

| Chemin | Rôle |
| --- | --- |
| `index.html` | La page entière : HTML, CSS et JavaScript, sans dépendance ni étape de build |
| `photo.png` | Portrait |
| `banner.jpg` | Fond du bandeau d'en-tête : photographie d'Andre Benz sur Unsplash, recadrée en 1920×600 et atténuée en CSS. La source pleine résolution reste hors du dépôt. |
| `diplomas/` | Certificats en PDF liés depuis la section Education |
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

1. **En préparation** (état par défaut) :
   ```html
   <span class="status">In preparation</span>
   ```
2. **Brouillon communicable** : le lecteur écrit pour l'obtenir.
   ```html
   <span class="status on-request">Draft &mdash; PDF on request</span>
   ```
3. **Publié** : déposer le PDF dans `papers/`, puis remplacer toute la ligne
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

contact@em-conseil-invest.fr · [LinkedIn](https://www.linkedin.com/in/elies-mlayah-69a542246/)

---

© 2026 Elies Mlayah. Le contenu de ce site (textes, photographie, justificatifs) est protégé et
n'est pas réutilisable sans autorisation.
