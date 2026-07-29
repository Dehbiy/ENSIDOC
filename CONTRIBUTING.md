# Contribuer au Guide ENSIMAG

Merci de vouloir contribuer ! Ce guide est maintenu par la communauté étudiante. Voici comment participer.

## Façons de contribuer

### 1. Corriger une information (le plus simple)

Chaque page du site a un bouton **Editer cette page** en haut à droite. Il t'amène directement sur GitHub pour proposer une correction.

### 2. Ajouter une nouvelle section ou page

1. **Fork** le dépôt sur GitHub

2. Clone ton fork en local :

3. Installe les dépendances avec `uv` :
   ```bash
   uv sync
   ```
4. Lance le serveur de développement :
   ```bash
   uv run mkdocs serve
   ```
5. Crée ou modifie tes fichiers Markdown dans `docs/`
6. Ajoute ta page au `nav:` dans `mkdocs.yml` si nécessaire
7. Commit + push + ouvre une **Pull Request**

### 3. Signaler une erreur ou suggérer du contenu

[Ouvre une issue](https://github.com/dehbiy/ENSIDOC/issues/new) en décrivant ce qui manque ou ce qui est incorrect.

---

## Structure des fichiers

```
docs/
├── index.md                    # Page d'accueil
├── administrative/             # Démarches (carte séjour, banque…)
├── vie-etudiante/              # Logement, transport, alimentation…
├── cours-scolarite/            # EDT, outils, organisation
├── associations-inp/           # BdE, associations, bureaux
└── faq/                        # Questions fréquentes
```

## Conventions de rédaction

- Langue : **français** (quelques termes en arabe ou anglais sont OK si contextuels)
- Ton : amical, direct, pratique — pas de jargon administratif inutile
- Format : Markdown standard + extensions Material (admonitions, tabs, checklists)
- Toujours citer les sources officielles quand possible
- Utiliser les admonitions pour les infos importantes :

```markdown
!!! tip "Conseil"
    Texte du conseil.

!!! warning "Attention"
    Texte d'avertissement.

!!! info "Information"
    Texte informatif.
```

## Template pour une nouvelle page

```markdown
---
title: Titre de la page
tags:
  - tag1
  - tag2
---

# Titre principal

Courte introduction.

---

## Section 1

Contenu...

---

*Page maintenue par la communauté — [Proposer une correction](...)*
```

---

Merci pour ta contribution ! 🙏
