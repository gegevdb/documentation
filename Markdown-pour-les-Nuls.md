# Markdown pour les Nuls - Guide Complet pour Philippo

## Table des matières
1. [Installation du plugin Markdown dans Chrome](#installation)
2. [Configuration du plugin](#configuration)
3. [Modifier l'ouverture par défaut](#ouverture-defaut)
4. [Différence entre texte ordinaire et code](#difference-texte-code)
5. [Créer un fichier Markdown](#creer-markdown)

---

## Installation du plugin Markdown dans Chrome {#installation}

### Étapes simples :

1. **Ouvrir le Chrome Web Store**
   - Allez sur https://chrome.google.com/webstore/category/extensions
   - Ou cliquez sur les 3 points en haut à droite de Chrome → Paramètres → Extensions

2. **Chercher "Markdown Viewer"**
   - Dans la barre de recherche, tapez "Markdown Viewer"
   - Plusieurs options existent, les plus populaires sont :
     - "Markdown Viewer" (par Gaj)
     - "Markdown Viewer Pro"

3. **Cliquer sur "Ajouter à Chrome"**
   - Confirmez en cliquant sur "Ajouter l'extension"
   - Une notification apparaît pour confirmer l'installation

4. **Accorder les permissions**
   - L'extension demande accès aux fichiers locaux
   - Cliquez sur l'icône de l'extension → Gérer les extensions
   - Activez "Accès aux URLs de fichiers"

✅ C'est fait ! Vous pouvez maintenant voir les fichiers `.md` formatés dans Chrome.

---

## Configuration du plugin {#configuration}

### Où trouver les paramètres :

1. **Clic droit sur l'icône de l'extension** (en haut à droite)
2. **Sélectionner "Options"**

### Options disponibles et leur utilité :

| Option | Utilité | Valeur par défaut |
|--------|---------|-------------------|
| **Thème** | Change l'apparence (clair/sombre) | Selon le système |
| **Zoom** | Augmente/diminue la taille du texte | 100% |
| **CSS personnalisé** | Permet de modifier l'apparence avec du code | Vide |
| **Markdown flavor** | Choisit le dialecte Markdown (CommonMark, GitHub...) | GitHub |
| **Activer les liens** | Permet de cliquer sur les liens | Activé |
| **Afficher le sommaire** | Génère automatiquement un index | Désactivé |

### Exemple de configuration recommandée :
- Thème : Dark (pour moins fatiguer les yeux)
- Zoom : 110% (plus lisible)
- Markdown flavor : GitHub (le plus complet)
- Afficher le sommaire : Activé (pratique pour grandes documentations)

---

## Modifier l'ouverture par défaut des fichiers .md avec Chrome {#ouverture-defaut}

### Sur Windows :

1. **Clic droit sur un fichier `.md`**
2. **"Ouvrir avec" → "Choisir une autre application"**
3. **Sélectionner "Google Chrome"**
4. **Cocher "Toujours utiliser cette application"**
5. **Cliquer "OK"**

### Sur macOS :

1. **Clic droit sur un fichier `.md`**
2. **"Ouvrir avec" → "Google Chrome"**
3. **Puis faire la même opération sur n'importe quel `.md`**
4. **Aller à "Informations" (Cmd+I)**
5. **Sélectionner Chrome dans "Ouvrir avec"**
6. **Cliquer "Modifier tout" (change pour tous les `.md`)**

### Sur Linux :

```bash
# Via terminal - remplacer google-chrome par chromium si nécessaire
xdg-mime default google-chrome.desktop text/markdown
```

✅ Désormais, tous les fichiers `.md` s'ouvrent automatiquement dans Chrome !

---

## Différence entre texte ordinaire et code formaté {#difference-texte-code}

### Texte ordinaire :
```
Ceci est un simple texte ordinaire. Il n'a aucune mise en forme spéciale. 
C'est juste du contenu lisible écrit en langage naturel, sans balises Markdown.
```

**Résultat :** 
Ceci est un simple texte ordinaire. Il n'a aucune mise en forme spéciale. C'est juste du contenu lisible écrit en langage naturel, sans balises Markdown.

---

### Texte avec formatage Markdown :
```markdown
# Titre Principal (Heading 1)
## Sous-titre (Heading 2)
### Sous-sous-titre (Heading 3)

**Voici du texte en gras** et *voici du texte en italique*.

Voici une liste à puces :
- Premier élément
- Deuxième élément
  - Sous-élément indentable
- Troisième élément

Voici une liste numérotée :
1. Première étape
2. Deuxième étape
3. Troisième étape

[Ceci est un lien vers Google](https://google.com)

Ci-dessous, du code inline : `print("Hello World")`

Et voici un bloc de code :
\`\`\`python
def bonjour():
    print("Bonjour Philippo!")
    return True

resultat = bonjour()
\`\`\`
```

**Résultat rendu :**

# Titre Principal (Heading 1)
## Sous-titre (Heading 2)
### Sous-sous-titre (Heading 3)

**Voici du texte en gras** et *voici du texte en italique*.

Voici une liste à puces :
- Premier élément
- Deuxième élément
  - Sous-élément indentable
- Troisième élément

Voici une liste numérotée :
1. Première étape
2. Deuxième étape
3. Troisième étape

[Ceci est un lien vers Google](https://google.com)

Ci-dessous, du code inline : `print("Hello World")`

Et voici un bloc de code :
```python
def bonjour():
    print("Bonjour Philippo!")
    return True

resultat = bonjour()
```

---

## Créer votre propre fichier Markdown {#creer-markdown}

### Les balises essentielles à connaître :

#### 1. **Titres**
```markdown
# Titre de niveau 1 (le plus grand)
## Titre de niveau 2
### Titre de niveau 3
#### Titre de niveau 4
##### Titre de niveau 5
###### Titre de niveau 6 (le plus petit)
```

#### 2. **Texte formaté**
```markdown
**Texte en gras** ou __texte en gras alternative__
*Texte en italique* ou _texte en italique alternative_
***Texte en gras ET italique***
~~Texte barré~~
```

#### 3. **Listes non-ordonnées**
```markdown
- Premier élément
- Deuxième élément
  - Sous-élément (indenter avec 2-4 espaces)
  - Autre sous-élément
- Troisième élément
```

#### 4. **Listes ordonnées**
```markdown
1. Première étape
2. Deuxième étape
3. Troisième étape
   1. Sous-étape
   2. Autre sous-étape
```

#### 5. **Liens et images**
```markdown
[Texte du lien](https://exemple.com)
[Lien avec titre](https://exemple.com "Titre au survol")
![Texte alternatif](chemin/vers/image.jpg)
```

#### 6. **Code**
```markdown
Code inline : `ceci est du code`

Bloc de code avec langage (pour coloration) :
\`\`\`python
print("Bonjour !")
\`\`\`

\`\`\`javascript
console.log("Bonjour !");
\`\`\`

\`\`\`bash
echo "Bonjour !"
\`\`\`
```

#### 7. **Citations/Blocs de citation**
```markdown
> Ceci est une citation.
> Elle peut s'étendre sur plusieurs lignes.
> 
> > Et on peut la imbriquer !
```

#### 8. **Lignes horizontales**
```markdown
---
***
___
```

#### 9. **Tableaux** (spécifique à GitHub Markdown)
```markdown
| En-tête 1 | En-tête 2 | En-tête 3 |
|-----------|-----------|-----------|
| Ligne 1   | Donnée    | Donnée    |
| Ligne 2   | Donnée    | Donnée    |
```

#### 10. **Échappement de caractères**
```markdown
Certains caractères nécessitent un backslash pour ne pas être interprétés :
\* \# \[ \]
```

---

### Exemple complet d'un fichier Markdown :

```markdown
# Mon Premier Projet - Guide

## Introduction

Bienvenue dans ce projet ! Voici les étapes pour **bien démarrer**.

## Installation

Suivez ces étapes :

1. Cloner le repository
   ```bash
   git clone https://example.com/repo.git
   ```
2. Installer les dépendances
3. Lancer l'application

## Fonctionnalités

- ✅ Fonctionnalité A
- ✅ Fonctionnalité B
- 🚀 Bientôt : Fonctionnalité C

## Auteur

Créé par **ꞬÉꞬÉ VDB** en 2026 (70ans hier).

[Visitez mon site](https://gégé.com)
```

---

## Conseils pratiques pour Philippo :

✨ **Astuces utiles :**

1. **Prévisualisation en temps réel**
   - Utilisez des éditeurs comme VS Code ou Markdown Preview Plus
   - Vous voyez le rendu au fur et à mesure

2. **Convertion en PDF**
   - Chrome : Imprimer (Ctrl+P) → Enregistrer au format PDF
   - Résultat : Un PDF bien formaté de votre markdown

3. **Compatibilité**
   - Markdown fonctionne partout : GitHub, Notion, Reddit, Discord...
   - Les balises universelles : `#`, `*`, `**`, `-`, etc.  
     (ouin moi j'ai clavier américain comment je fais ## hashtag ## ¿¿¿

4. **Validation**
   - Vous pouvez vérifier votre markdown sur : https://commonmark.org/try/

5. **Bonnes pratiques**
   - Commencez par un `# Titre`
   - Utilisez des espaces entre les sections
   - Gardez un indentation cohérente pour les listes
   - Préférez `---` pour les lignes horizontales

---

## Récapitulatif

| Tâche | Étapes simples |
|-------|---|
| **Installer plugin** | Chrome Web Store → Chercher → Ajouter |
| **Configurer** | Clic droit extension → Options → Régler thème/zoom |
| **Ouvrir .md par défaut** | Clic droit fichier → Ouvrir avec → Chrome → Toujours utiliser |
| **Créer Markdown** | Mémoriser 5-6 balises clés (`#`, `**`, `-`, `` ` ``, etc.) |

✅ **Vous êtes maintenant un ninja du Markdown !** 🥋

---

*Créé pour Philippo - Guide complet Markdown - gegevdb ©2026*

