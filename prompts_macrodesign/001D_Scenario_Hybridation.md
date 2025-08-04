# 🧠 Prompt `001D` – Scénario et hybridation

## 🎯 Objectif du prompt

Ce prompt vous permet de choisir la **structure globale** de votre parcours de formation.  
Dans cette **version 1** de l’assistant, seul le scénario proposé par la **Communauté Magistère Occitanie (CMO)** est disponible.

Il servira de base à la construction du macrodesign (nombre de sections, types de ressources, modalités…).

> 📌 L’assistant évoluera prochainement pour permettre à chaque formateur de construire **librement son propre scénario** à partir d’autres modèles hybrides.

---

## ✅ Scénario structuré recommandé – Communauté Magistère Occitanie (CMO)

- Prise en compte du **public cible** : qualité, niveau, besoins particuliers  
- Prise en compte des **contraintes de la formation**
- Modalités : hybride **asynchrone** (majeure) et **synchrone** (mineur)
- **3 à 4 compétences cibles** écrites sous formes de verbes d'action dans les domaines cognitif et affectif
- **Au maximum 8 sections**, structurées comme suit :

| N° | Type de section               | Contenu attendu                                                                 | Modalités prévues   |
|----|-------------------------------|----------------------------------------------------------------------------------|---------------------|
| 1  | **Accueil**                   | Présentation générale de la formation, objectifs, déroulé                        | Asynchrone          |
| 2  | **Section d’apprentissage 1** | Compétence 1 – Ressource, activité(s), référentiel, badge, discussion associée   | Asynchrone          |
| 3  | **Section d’apprentissage 2** | Compétence 2 – Idem                                                              | Asynchrone          |
| 4  | **Section d’apprentissage 3** | Compétence 3 – Idem                                                              | Asynchrone          |
| 5  | **Section d’apprentissage 4** *(si 4e compétence)* | Idem (optionnelle)                                     | Asynchrone          |
| 6  | **Classe virtuelle (BBB)**    | Point intermédiaire, accompagnement à la demande, approfondissement              | Synchrone           |
| 7  | **Forum général**             | Discussions regroupées par compétence                                            | Asynchrone          |
| 8  | **Évaluation de satisfaction**| Bilan à court, moyen et long terme                                               | Asynchrone          |

- **Durée de 3h maximum**  
- **Poids total de 512 Mo maximum**

---

## ❓Souhaitez-vous adopter ce scénario comme base de votre parcours ?

☐ Oui, je valide le scénario **Communauté Magistère Occitanie**  
☐ Non, je souhaite utiliser un autre scénario libre (non disponible dans cette version)

> ⚠️ *Si vous ne validez pas le scénario CMO, l’assistant ne pourra pas encore vous accompagner dans la construction d’un scénario alternatif.*  
> Vous pouvez cependant consulter les ressources ci-dessous pour construire votre propre modèle.  
> Ce fonctionnement évoluera dans la **version 2** de l’assistant.

---

## 📘 Ressources complémentaires (consultation libre)

- 📎 `02_ressources_formateur/02_Modèles_pédagogiques_et_théoriques/032_HySup_ABC_Scenarios.md`  
  → Comparatif de scénarios hybrides alternatifs
- 🧪 [Test Carenn – Quel formateur êtes-vous ?](http://www.pedagosup.fr/carenn/#)  
  → Pour identifier votre profil de formateur

---

## 🔁 Synthèse à valider

Merci de valider la synthèse suivante avant de poursuivre :

```yaml
scenario_souhaite:
  reference: "CMO"
  inspiration: ./032_HySup_ABC_Scenarios.md
  scenario_libre_disponible_version2: false
  modalites_par_section:
    - Accueil : Asynchrone
    - Apprentissage 1 : Asynchrone
    - Apprentissage 2 : Asynchrone
    - Apprentissage 3 : Asynchrone
    - Apprentissage 4 : Asynchrone
    - Classe virtuelle : Synchrone
    - Forum général : Asynchrone
    - Évaluation de satisfaction : Asynchrone
```

☐ Oui, je valide cette synthèse  
☐ Non, je souhaite corriger certains éléments

---

✅ Le bloc YAML validé sera repris automatiquement dans le prompt `001E_Competences_Visées.md`.
