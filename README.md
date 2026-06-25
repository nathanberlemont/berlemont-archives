# Berlemont — Archives

Portfolio personnel de Nathan Berlemont — photographie, architecture d'intérieur, et autres travaux.

---

## Ajouter des images

Place tes images dans le dossier `images/` avec les noms suivants :

| Catégorie | Nommage suggéré |
|---|---|
| Photographie | `photo-01.jpg`, `photo-02.jpg`, ... |
| Architecture d'intérieur | `archi-01.jpg`, `archi-02.jpg`, ... |
| Autres | `autre-01.jpg`, `autre-02.jpg`, ... |

Pour chaque nouvelle image, ajoute un bloc dans `index.html` à l'intérieur de `<div id="galleryGrid">` :

```html
<div class="gallery-item" data-category="photographie" data-title="Ton titre">
  <img src="images/photo-05.jpg" alt="Description" loading="lazy" />
  <div class="gallery-overlay">
    <div class="gallery-meta">
      <span class="gallery-category">Photographie</span>
      <span class="gallery-title">Ton titre</span>
    </div>
  </div>
</div>
```

Les valeurs possibles pour `data-category` : `photographie` · `architecture` · `autres`

---

## Déployer sur GitHub Pages

1. **Crée un compte GitHub** sur [github.com](https://github.com) si tu n'en as pas.

2. **Crée un nouveau dépôt** : bouton `+` → *New repository*
   - Nom : `berlemont-archives` (ou ce que tu veux)
   - Visibilité : **Public**
   - Ne coche rien d'autre, clique *Create repository*

3. **Upload les fichiers** : sur la page du dépôt vide, clique *uploading an existing file*
   - Glisse tout le contenu du dossier `berlemont-archives/` (le fichier `index.html`, le dossier `images/`, ce `README.md`)
   - Clique *Commit changes*

4. **Active GitHub Pages** :
   - Va dans *Settings* → *Pages* (dans le menu de gauche)
   - *Source* : Deploy from a branch → branche `main`, dossier `/ (root)`
   - Clique *Save*

5. **Ton site est en ligne** en quelques minutes à l'adresse :
   ```
   https://TON-PSEUDO-GITHUB.github.io/berlemont-archives/
   ```

---

## Personnaliser les textes

Dans `index.html`, cherche ces sections pour modifier les contenus :

- **Titre hero** : `Archives<br /><em>&amp; travaux</em>`
- **Description** : le paragraphe `class="hero-desc"`
- **Lien Instagram** dans le footer : `href="https://instagram.com/_nathan_design_berlemont"`

---

*Site conçu pour être léger, rapide, et sans dépendances externes (hors polices Google Fonts).*
