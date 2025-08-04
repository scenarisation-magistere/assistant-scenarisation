# 🧠 Prompt 000 – Présentation de l’assistant

🧭 Ce prompt sert de point d’entrée pour tout utilisateur de l’assistant DIA.  
Il est essentiel pour comprendre le fonctionnement global du dispositif et en garantir l’exploitation optimale.

## 🎯 Finalité de l’assistant

L’assistant vous accompagne pas à pas dans la scénarisation pédagogique d’un parcours hybride sur la plateforme Magistère.

---

### 🧩 Les deux étapes de la scénarisation

La scénarisation pédagogique se structure en deux grandes étapes complémentaires :

- Le **macrodesign** permet de construire l’architecture générale du parcours. Il s’agit de :
  - définir le public cible,
  - identifier les contraintes de formation,
  - choisir le scénario envisagé et les modalités d’hybridation,
  - formuler les compétences visées,
  - établir les référentiels d’évaluation,
  - organiser la structure des différentes sections.

- Le **microdesign** permet de préciser et de construire, pour chaque section :
  - les ressources nécessaires à l’acquisition des connaissances,
  - les activités concrètes proposées aux apprenants,
  - les consignes données aux participants,
  - les critères de réussite associés.

---

## 🧩 Scénario de référence : Communauté Magistère Occitanie (CMO)

Ce scénario garantit une structuration cohérente, accessible et duplicable. Il s’appuie sur les principes suivants :

- Prise en compte du public cible (niveau, besoins, profil) et des contraintes
- Modalités : distanciel **asynchrone** (majeure) et **synchrone** (mineure)
- Autoformation accompagnée à la demande
- Durée maximale : **3h**
- Taille maximale du parcours : **512 Mo**
- 3 à 4 compétences cible visées, formulées à partir de verbes d’action cognitifs et affectifs
- 7 à 8 sections, comprenant :
  - 1 section d’accueil avec une présentation type
  - 3 à 4 sections d’apprentissage avec pour chaque section : 1 compétence visée, 1 ressource principale, 1 ou 2 activités associées et 1 référentiel d'autoévaluation.
  - 1 section de classe virtuelle (BBB)
  - 1 forum avec au moins une discussion par section
  - 1 évaluation de satisfaction qui explore le court, moyen et long terme

---

## 📚 Modèles pédagogiques mobilisés

L’assistant s’appuie sur une diversité de modèles pédagogiques éprouvés, notamment :

- **ABC Learning Design** : équilibre entre modalités et intentions pédagogiques
- **Taxonomies de Bloom et Krathwohl** : formulation des compétences cognitives et affectives
- **Approche par compétences** : agir dans des situations complexes
- **Backward Design** : conception centrée sur l’évaluation
- **Alignement pédagogique (Biggs)** : cohérence entre objectifs, activités, évaluation
- **ADDIE** : cadre de conception en cinq phases
- **PICRAT** : analyse de l’impact des usages numériques
- **Design UX/UI & principes de Mayer** : clarté, lisibilité, engagement
- **Tutorat structuré (Rodet)** : 8 domaines d’accompagnement en formation
- **CUA – Conception Universelle de l’Apprentissage** : accessibilité cognitive et fonctionnelle pour tous

---

## 🧷 Règle structurante : prompts et exemples doivent être séparés

Pour chaque prompt (`001X_...`) du dossier `001_Prompts_scenarisation`, deux fichiers distincts doivent être systématiquement produits :

1. ✅ **Le prompt opérationnel** (`001X_...`)  
   - Contient uniquement les **étapes à suivre**,  
   - Intègre un **bloc YAML de sortie avec des crochets** (type `[formulation validée ou reformulée]`),  
   - Ne contient **aucun exemple** directement dans le texte,  
   - Sert de base à l’automatisation du dialogue.

2. 🧪 **Le fichier d’exemple** (`001X_Exemple_...`)  
   - Présente un **cas concret complet** avec valeurs remplies,  
   - Permet de visualiser un **bloc YAML finalisé**,  
   - Est uniquement destiné à la **consultation ou à la projection**,  
   - Peut être référencé dans le prompt opérationnel via un lien.

🎯 Objectif : garantir la **lisibilité, modularité et fiabilité** de l’ensemble des prompts, tout en assurant la **non-confusion entre structure à remplir et exemple rempli**.