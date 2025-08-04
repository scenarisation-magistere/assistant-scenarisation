# 🧠 Prompt `001C` – Contraintes de la formation

## 🎯 Objectifs du prompt

- Préciser les contraintes temporelles, organisationnelles et techniques  
- Servir de base pour orienter la scénarisation macro

Les informations recueillies ici permettent à l’assistant d’ajuster la structure globale de la formation aux réalités du terrain, en respectant le cadre proposé par le scénario CMO.

---

## 🧭 Formulaire à compléter

Merci d’indiquer les paramètres suivants concernant la formation à concevoir :

### 1. Type de parcours  
`[type_parcours]`  
☐ Création d’un nouvel espace  
☐ Migration d’un parcours existant  
> *Si migration : voir le [Grain Magistère – Migration de parcours](https://toulouse.magistere.apps.education.fr/course/view.php?id=398)*

---

### 2. Modalités hybrides prévues  
`[modalites_hybridation]`  
☐ Distanciel asynchrone (majeur) + distanciel synchrone (mineur) — *Recommandé CMO*  
☐ Autre – précisez : `[à compléter]`

---

### 3. Temps estimé de la formation  
`[temps_total]`  
☐ Moins de 3h — *Recommandé par la CMO*  
☐ Entre 3h et 6h  
☐ 6h ou plus

---

### 4. Autonomie souhaitée des participants  
`[autonomie]`  
☐ Autoformation (sans accompagnement)  
☐ Formation tutorée (accompagnement ponctuel) — *Recommandé par la CMO*

---

### 5. Modalités d’animation  
`[animation]`  
☐ Formation animée par un seul intervenant  
☐ Coanimation prévue (2 intervenants ou plus)

---

### 6. Contraintes de calendrier  
`[calendrier]`  
☐ Début d’année scolaire  
☐ 2e trimestre  
☐ Fin d’année  
☐ Période imposée – précisez : `[à compléter]`

---

### 7. Contraintes d’horaires (temps synchrone)  
`[horaires]`  
☐ Sur temps de travail (journée / service)  
☐ Hors temps de travail (soir, à partir de 17h00)  
☐ Horaires précis à définir – précisez : `[à compléter]`

---

### 8. Nombre estimé de participants  
`[nombre_participants]`  
☐ Moins de 10 personnes  
☐ Entre 10 et 20 personnes  
☐ Entre 20 et 30 personnes  
☐ Entre 30 et 40 personnes  
☐ Autoformation (public illimité)

---

### 9. Exigences institutionnelles particulières  
`[exigences_institutionnelles]`  
☐ Oui – à préciser : `[à compléter]`  
☐ Non

---

### 10. Restrictions techniques connues  
`[restrictions_techniques]`  
☐ Oui – à préciser : `[à compléter]`  
☐ Non

---

## 🔁 Synthèse proposée à valider

Merci de valider la synthèse suivante avant de poursuivre :

```yaml
contraintes_formation:
  type_parcours: "[type_parcours]"
  hybridation: "[modalites_hybridation]"
  temps_total: "[temps_total]"
  autonomie: "[autonomie]"
  animation: "[animation]"
  calendrier: "[calendrier]"
  horaires: "[horaires]"
  nombre_participants: "[nombre_participants]"
  exigences_institutionnelles: "[exigences_institutionnelles]"
  restrictions_techniques: "[restrictions_techniques]"
  exemple_associe: "001C_Exemple_Contraintes_Formation.md"
```

- ☐ Oui, je valide cette synthèse  
- ☐ Non, je souhaite corriger certains éléments

---

## 🔁 En cas de correction

Si vous avez coché “Non”, veuillez indiquer les éléments à corriger :

- ☐ Type de parcours  
- ☐ Modalités hybrides prévues  
- ☐ Temps estimé de la formation  
- ☐ Autonomie souhaitée  
- ☐ Modalités d’animation  
- ☐ Contraintes de calendrier  
- ☐ Contraintes horaires  
- ☐ Nombre estimé de participants  
- ☐ Exigences institutionnelles  
- ☐ Restrictions techniques

Une nouvelle synthèse vous sera proposée avec les éléments mis à jour.  
Le bloc YAML final sera mis à jour à chaque itération jusqu’à validation explicite.

---

✅ Le bloc YAML validé à la fin de ce prompt sera automatiquement repris dans le prompt suivant `001D_Scenario_Hybridation.md`.
