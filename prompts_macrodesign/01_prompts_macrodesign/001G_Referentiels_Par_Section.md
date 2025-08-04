# 🧭 Prompt `001G` – Référentiels d’auto-évaluation par section

## 🎯 Objectif

Générer un **référentiel d’auto-évaluation clair, progressif et accessible** pour chaque section d’apprentissage, à partir des compétences définies dans le prompt `001F`.

Ce prompt s’inscrit dans une double logique pédagogique :
- **Alignement pédagogique** (Biggs) : cohérence entre objectifs, activités et évaluation  
- **Backward Design** (Wiggins & McTighe) : partir des résultats attendus pour concevoir la formation

> 📌 L’ordre des compétences dans le bloc `ordre_competences` détermine l’ordre des sections du parcours  
> (section 1 = 1ʳᵉ compétence, etc.)

---

## 📐 Structure type du scénario (rappel CMO)

| Section | Type                       | Contenu attendu                                      |
|---------|----------------------------|-------------------------------------------------------|
| 1       | Accueil                    | Objectifs, déroulé, contact                           |
| 2-5     | Section d’apprentissage    | Compétence + ressource + activité(s) + référentiel   |
| 6       | Classe virtuelle (BBB)     | Accompagnement, approfondissement                    |
| 7       | Forum                      | Discussions par compétence                           |
| 8       | Évaluation de satisfaction | Retours court, moyen et long terme                   |

---

## ⚙️ Générations automatiques prises en charge par l’assistant

L’assistant DIA effectue automatiquement les opérations suivantes :

- 💬 Génère pour chaque compétence un **référentiel à 4 degrés de progression**, incluant :
  - un **indicateur qualitatif** (type : *Je suis capable de…*)  
  - un **indicateur quantitatif** (type : score, fréquence, action réalisée)  
- ♿ Propose des **adaptations pédagogiques (CUA)** en croisant chaque compétence avec les besoins spécifiques présents dans le bloc YAML validé `public_cible.besoins_specifiques`
- 🏅 Active un **badge de validation** si le participant atteint le **degré 3**

> ⚠️ L’assistant n’utilise **que les besoins spécifiquement validés** dans le bloc final YAML issu du prompt `001B_Public_Cible.md`.  
> Il ne s’appuie pas sur la liste complète du formulaire initial, mais uniquement sur les valeurs comme :
> ```yaml
> public_cible:
>   besoins_specifiques:
>     - "Fatigabilité importante"
>     - "Troubles des fonctions exécutives"
> ```

---

## 📤 Référentiels d’auto-évaluation par section

| Section d’apprentissage | Compétence visée                             | Adaptation CUA (si besoin)                           | Degré 1 – Je débute      | Degré 2 – Je progresse     | Degré 3 – Je suis autonome   | Degré 4 – Je maîtrise avec aisance | Badge                   |
|-------------------------|---------------------------------------------|------------------------------------------------------|---------------------------|----------------------------|-------------------------------|------------------------------------|--------------------------|
| Section 2               | [formulation compétence 1]                  | [Adaptation issue des besoins spécifiques si présents] | • Qual. … <br>• Quant. … | • … <br>• …               | • … <br>• …                  | • … <br>• …                         | oui (si degré 3 atteint) |
| Section 3               | [formulation compétence 2]                  | [Adaptation issue des besoins spécifiques si présents] | • … <br>• …              | • … <br>• …              | • … <br>• …                  | • … <br>• …                         | oui (si degré 3 atteint) |
| Section 4               | [formulation compétence 3]                  | [Adaptation issue des besoins spécifiques si présents] | • … <br>• …              | • … <br>• …              | • … <br>• …                  | • … <br>• …                         | oui (si degré 3 atteint) |
| Section 5               | [formulation compétence 4] *(si présente)*  | [Adaptation issue des besoins spécifiques si présents] | • … <br>• …              | • … <br>• …              | • … <br>• …                  | • … <br>• …                         | oui (si degré 3 atteint) |

---

## 📦 Bloc YAML à transmettre

Ce bloc est automatiquement généré et pourra être réutilisé dans le prompt `001H` pour la scénarisation détaillée des contenus par section.

```yaml
referentiels_par_section:
  - section: 2
    competence: "[formulation compétence 1]"
    adaptation_CUA: "[si besoin identifié à partir de public_cible]"
    badge: "oui (si degré 3 atteint)"
    niveaux:
      - degre: 1
        observable_qualitatif: "[Je suis capable de…]"
        observable_quantitatif: "[score, action, fréquence…]"
      - degre: 2
        observable_qualitatif: "[...]"
        observable_quantitatif: "[...]"
      - degre: 3
        observable_qualitatif: "[...]"
        observable_quantitatif: "[...]"
      - degre: 4
        observable_qualitatif: "[...]"
        observable_quantitatif: "[...]"

  - section: 3
    competence: "[formulation compétence 2]"
    adaptation_CUA: "[...]"
    badge: "oui (si degré 3 atteint)"
    niveaux:
      - degre: 1
        observable_qualitatif: "[...]"
        observable_quantitatif: "[...]"
      ...
```

---

## 📚 Ressources associées
- [000_Prompt_Assistant.md] – Présentation globale du fonctionnement de l’assistant  
- [001A_Presentation_Macrodesign.md] – Règles du macrodesign et articulation des prompts  
- [001B_Public_Cible.md] – Profil du public et besoins spécifiques validés  

---

## ✅ Étapes suivantes

Le bloc `referentiels_par_section` sera injecté dans le prompt `001H` (contenus par section) pour aligner les intentions pédagogiques, les ressources et les activités avec les niveaux d’atteinte de chaque compétence.

