# Projet : Dimensionnement de Serres Agricoles (EN 13031 + Eurocodes)

Ce projet vise à modéliser et automatiser le dimensionnement des serres agricoles selon la norme **EN 13031-1** et les **Eurocodes (EN 1991-1-4)** grâce à des diagrammes **PlantUML** générés automatiquement et déployés via GitHub Pages.

---

## 🎯 Objectif

- Faciliter le **dimensionnement normatif des portiques bi-versants** avec traçabilité vers les articles Eurocodes.  
- Automatiser le calcul des actions climatiques (vent, neige).  
- Générer des diagrammes interactifs avec **PlantUML**.  
- Créer des liens cliquables vers les articles des normes.  
- Assurer un suivi de version et une collaboration fluide via GitHub.

---

## 🚀 Fonctionnalités principales

- **Diagrammes UML en PlantUML** pour la modélisation complète.  
- **Génération automatique** des diagrammes SVG via GitHub Actions.  
- **Déploiement des SVG** en ligne via GitHub Pages (consultation facile).  
- **Références claires** aux normes et articles Eurocodes.  
- **Workflow CI/CD** pour automatiser génération et déploiement.  
- Collaboration simplifiée avec fork, branches, PR.

---

## 📁 Structure du projet

| Dossier/Fichier              | Description                                      |
|-----------------------------|------------------------------------------------|
| `.github/workflows/`         | Workflows GitHub Actions pour CI/CD             |
| `diagrams/`                 | Fichiers sources `.puml` des diagrammes          |
| `docs/`                     | Diagrammes SVG générés automatiquement            |
| `pdf/`                      | Copies PDF des normes utilisées                    |
| `README.md`                 | Documentation principale du projet                  |

---

## 🌐 1. Accéder aux diagrammes en ligne

Les diagrammes sont automatiquement générés à partir des fichiers `.puml` dans `diagrams/`  
et déployés sur GitHub Pages.  

👉 [Voir les diagrammes sur GitHub Pages](https://apesseu.github.io/serre-agricole-en13031/)

---

## 💻 2. Travailler localement

Pour étudier ou modifier les diagrammes :  

```bash
git clone https://github.com/apesseu/serre-agricole-en13031.git
cd serre-agricole-en13031
```
- Modifiez les fichiers .puml dans diagrams/.
- Vous pouvez générer les SVG localement avec PlantUML (Java requis) 

---

## 🤝 3. Collaborer et contribuer

1. Forkez ce dépôt sur votre compte GitHub.

2. Ajoutez ou modifiez les fichiers .puml dans diagrams/.

3. Commitez et poussez vos changements sur votre branche.

4. Ouvrez une Pull Request vers main ou test-plantuml.

Chaque PR déclenche :

    - La génération automatique des SVG.

    - La mise à jour du site GitHub Pages avec les diagrammes mis à jour.

---

## 🔧 4. Détails du workflow CI/CD

- Branches surveillées : main et test-plantuml.

- Actions réalisées :

    - Téléchargement de PlantUML et installation de Java + Graphviz.

    - Recherche des fichiers .puml dans diagrams/.

    - Génération des diagrammes SVG dans docs/.

    - Création d’une page index.html listant tous les SVG.

    - Déploiement automatique sur la branche gh-pages via GitHub Pages.

---

## 📜 5. Références normatives

- EN 13031-1 – Serres agricoles.

- Eurocode EN 1991-1-4 – Actions du vent.

Les diagrammes font référence aux articles de ces normes pour un suivi clair.
