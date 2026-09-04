# elies-droid.github.io

Site de présentation personnelle d'**Elies Mlayah**, fondateur d'EM Conseil Invest (conseil en
investissement et stratégie patrimoniale) et Sales Specialist France chez Certu Systems EMEA.

**En ligne : https://elies-droid.github.io/**

Parcours professionnel, formations et certifications avec les justificatifs consultables en PDF.

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

Pour publier un article : décommenter la section `writing` et sa ligne d'onglet dans `index.html`,
puis dupliquer un bloc `<article class="paper">`.

## Contact

contact@em-conseil-invest.fr · [LinkedIn](https://www.linkedin.com/in/elies-mlayah-69a542246/)

---

© 2026 Elies Mlayah. Le contenu de ce site (textes, photographie, justificatifs) est protégé et
n'est pas réutilisable sans autorisation.
