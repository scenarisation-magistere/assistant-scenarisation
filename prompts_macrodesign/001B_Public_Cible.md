# 🧠 Prompt `001B` – Public cible

## 🎯 Objectif du prompt

Ce prompt vise à déterminer les caractéristiques du public cible de votre formation.  
Ces éléments permettront à l’assistant d’adapter finement ses propositions pédagogiques.

---

## 🧭 Formulaire à compléter

Merci de renseigner les éléments suivants :

### 1. Titre de la formation (ou projet de titre)  
`[titre_formation]`

> _Exemple : Développer les compétences orales en classe hétérogène_

---

### 2. Objectif général de la formation  
`[objectif_general]`

> _Exemple : Accompagner les enseignants à concevoir et animer des activités permettant aux élèves de s’exprimer oralement avec confiance et clarté._

---

### 3. Quel est le type de public visé ?  
`[type_de_public]`  
☐ Enseignants 1er degré  
☐ Enseignants 2d degré  
☐ Formateurs académiques  
☐ Formateurs INSPE / chercheurs  
☐ Inspecteurs  
☐ Équipes pluri-catégorielles  
☐ Autre (à préciser)

---

### 4. Quel est le niveau d’expertise global du public visé ?  
`[niveau_expertise]`  
☐ Débutant  
☐ Intermédiaire  
☐ Avancé  
☐ Expert ou formateur confirmé  
☐ Je ne sais pas encore

---

### 5. Le groupe est-il homogène ou hétérogène ?  
`[profil_groupe]`  
☐ Groupe homogène (mêmes profils, mêmes besoins)  
☐ Groupe hétérogène  
☐ Je ne sais pas encore

---

### 6. Des besoins spécifiques sont-ils connus pour ce public ?  
`[besoins_specifiques]`  
☐ Aucun besoin identifié  
☐ Troubles sensoriels (vue, audition…)  
☐ Troubles de la compréhension / expression écrite ou orale  
☐ Troubles des fonctions exécutives ou de l’attention  
☐ Fatigabilité ou surcharge mentale  
☐ Préférence pour certaines modalités (oral, écrit, visuel…)  
☐ Autre (à préciser)

---

## 🔁 Synthèse proposée à valider

Merci de valider la synthèse suivante avant de poursuivre :

```yaml
public_cible:
  type: [ "[type_de_public]" ]
  profil: "[profil_groupe]"
  niveau_expertise: "[niveau_expertise]"
  besoins_specifiques:
    - "[besoin_1]"
    - "[besoin_2]"
  recommandations:
    - "[à compléter ou à reformuler en fonction du profil et des besoins]"
contexte_formation:
  titre: "[titre_formation]"
  objectif_general: "[objectif_general]"
  exemple_associe: "001B_Exemple_Public_Cible.md"
```

- ☐ Oui, je valide cette synthèse  
- ☐ Non, je souhaite corriger certains éléments

---

## 🔁 En cas de correction

Si vous avez coché “Non”, veuillez indiquer les éléments à corriger :

- ☐ Le titre de la formation  
- ☐ L’objectif général  
- ☐ Le type de public  
- ☐ Le niveau d’expertise  
- ☐ Le profil du groupe  
- ☐ Les besoins spécifiques

Une nouvelle synthèse vous sera proposée avec les éléments mis à jour.  
Le bloc YAML final sera mis à jour à chaque itération jusqu’à validation explicite.

---

✅ Le bloc YAML validé à la fin de ce prompt sera automatiquement repris dans le prompt suivant `001C_Contraintes_Formation.md`.
