# 🧠 Prompt `001A` – Présentation du macrodesign

🧭 Ce prompt sert à **présenter la structure complète du macrodesign** dans l’assistant DIA.  
Il est destiné à **informer le formateur** sur les étapes, les règles et les principes qui guident la scénarisation pédagogique de son espace de formation sur Magistère.

---

## 🎯 Objectif du macrodesign

Le macrodesign permet de **concevoir l’architecture générale** du parcours de formation, selon une logique progressive, cohérente et modulaire.

Il structure la formation en **sections**, autour de **compétences clairement définies**, en garantissant l’articulation entre :
- les objectifs pédagogiques,
- les activités proposées,
- les modalités d’évaluation,
- l’accompagnement des apprenants.

---

## 📐 Le scénario de référence : modèle CMO

Le macrodesign proposé s’appuie sur le scénario-type de la **Communauté Magistère Occitanie (CMO)** :

- 1 section d’accueil  
- 3 à 4 sections d’apprentissage (1 compétence par section)  
- 1 section de classe virtuelle (renforcement / accompagnement)  
- 1 section de forum général  
- 1 section d’évaluation de satisfaction

Contraintes :
- 3 à 4 compétences maximum  
- Durée maximale : 3 heures  
- Taille maximale : 512 Mo  
- Modalité : hybride, à dominante asynchrone  
- Autoformation accompagnée (tutorat à la demande)

---

## 🔁 Enchaînement des prompts de macrodesign

| Code | Intitulé du prompt | Fonction |
|------|--------------------|----------|
| `001B` | Public cible | Identifier les publics visés et leurs besoins |
| `001C` | Contraintes | Identifier les contraintes de conception et de diffusion |
| `001D` | Scénario souhaité | Définir le format hybride et les modalités d’accompagnement |
| `001E` | Formulation des compétences | Créer jusqu’à 4 compétences visées |
| `001F` | Organisation des compétences | Réorganiser les compétences dans un ordre pédagogique cohérent |
| `001G` | Référentiels par section | Générer les référentiels d’autoévaluation par section |
| `001H` | Contenus par section | Définir les intentions, ressources, activités, discussions, badges |
| `001I` | Macrodesign global | Compiler toutes les sections dans un tableau synthétique |
| `001J` | Tutorat – anticipation | Définir les modalités d’accompagnement, relance, suivi différencié |

---

## 🧩 Fonction des blocs YAML

Chaque prompt opérationnel produit un **bloc YAML** qui permet :
- le passage fluide à l’étape suivante,
- la construction progressive du macrodesign final,
- la génération automatisée d’un espace Magistère aligné sur le scénario CMO.

📌 Ces blocs sont **lisibles et réutilisables par tout prompt ultérieur**, y compris dans le microdesign.

---
> ⚠️ **Important – À lire avant de commencer**  
>
> Une fois que vous débutez le processus de macrodesign, vous devez impérativement aller **jusqu’à la validation finale et l’export du fichier YAML**.  
> Ce fichier est **indispensable** pour enchaîner sur le microdesign.  
>
> 🔒 Si vous interrompez le processus en cours de route (par exemple en fermant la session ou en changeant de sujet), **aucune donnée ne pourra être conservée** ni réutilisée automatiquement.
>
> 💾 Pensez à **exporter et sauvegarder localement** le fichier final dès sa génération, afin de pouvoir le réimporter plus tard dans le prompt `002A` du microdesign.

---

## 📂 À savoir

- Ce prompt est **informel et non interactif** : il ne génère pas de tableau ni de YAML.
- Il peut être rappelé à tout moment pour **se repérer dans la progression**.
- Il fonctionne en **parallèle** avec le fichier `002A_Presentation_Microdesign.md` qui présente la structuration d’une seule section.