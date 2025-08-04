# 🧭 Prompt `001F` – Ordre et contenus par section (scénario CMO)

## 💡 Objectif

Organiser les compétences dans un ordre pédagogique progressif, cohérent avec :
- la logique d’alignement pédagogique (Biggs),
- la progressivité des niveaux cognitifs et affectifs (Bloom & Krathwohl),
- les intentions pédagogiques ABC Learning Design.

🎯 Cette articulation constitue le cœur de la scénarisation pédagogique.

> ℹ️ **Remarque importante** :  
> L’ordre retenu pour les compétences détermine **directement l’ordre des sections d’apprentissage**.  
> La compétence placée en 1ʳᵉ position alimentera la **section 1**, la 2ᵉ position la **section 2**, etc.  
> Le code (ex. `C3`) est un identifiant technique : seule la position dans la liste compte pour les sections.

---

## 🧾 Compétences définies

Les compétences listées ci-dessous sont automatiquement extraites du bloc YAML validé à la fin du prompt `001E_Competences_Visées.md`, sous la clé `formulations_competences`.

Elles sont reprises **telles quelles**, sans justification pédagogique, ni reformulation.

```yaml
formulations_competences:
  - "[formulation compétence 1 validée ou reformulée]"
  - "[formulation compétence 2 validée ou reformulée]"
  - "[formulation compétence 3 validée ou reformulée]"
  - "[formulation compétence 4 validée ou reformulée]"
```

## 📚 Références pédagogiques mobilisées

| Référence pédagogique              | Fonction dans cette étape                                                  |
|-----------------------------------|----------------------------------------------------------------------------|
| Alignement pédagogique (Biggs)   | Garantir la cohérence entre objectifs, activités et évaluation            |
| Taxonomies de Bloom & Krathwohl  | Classer les compétences selon leur niveau de difficulté cognitive et affective |
| ABC Learning Design               | Orienter les intentions pédagogiques et équilibrer les modalités d’apprentissage |

---

## 📋 Étapes à suivre

### 🧱 Étape 1 – Proposition d’un ordre pédagogique

L’assistant vous propose un ordre pédagogique initial, fondé sur :

- la complexité croissante des compétences (Bloom & Krathwohl),
- une entrée accessible pour favoriser l’engagement,
- une montée progressive vers des compétences plus complexes ou réflexives.

```yaml
ordre_propose:
  - code: C1
    formulation: "[formulation compétence 1]"
  - code: C3
    formulation: "[formulation compétence 3]"
  - code: C2
    formulation: "[formulation compétence 2]"
  - code: C4
    formulation: "[formulation compétence 4]"
```

---

### 🧠 Étape 2 – Justification par l’assistant

Voici la logique qui a guidé l’ordre proposé :

- **C1** : introduit les bases, engage sans difficulté technique.
- **C3** : renforce l’autonomie à travers une tâche pratique.
- **C2** : permet de transférer dans une autre situation.
- **C4** : mobilise une posture plus réflexive en fin de parcours.

---

### 📝 Étape 3 – Ordre retenu par le formateur

Vous pouvez conserver l’ordre proposé ou le modifier ci-dessous.

```yaml
ordre_retenu:
  - code: C1
    formulation: "[formulation compétence 1]"
    justification: "[expliquer pourquoi cette compétence en 1re position]"
  - code: C3
    formulation: "[formulation compétence 3]"
    justification: "[justification pour cette position]"
  - code: C2
    formulation: "[formulation compétence 2]"
    justification: "[...]"
  - code: C4
    formulation: "[formulation compétence 4]"
    justification: "[...]"
```

---

### ✅ Étape 4 – Validation finale

- [ ] Oui, je valide cet ordre pédagogique pour la suite du parcours  
- [ ] Non, je souhaite le modifier à nouveau

✏️ Si non, précisez ce que vous souhaitez modifier :  
__________________________________________________________  
__________________________________________________________

---

> 🔄 **Correspondance avec les sections d’apprentissage**  
> Lors de l’export du bloc YAML ci-dessous, **l’ordre d’apparition des compétences** déterminera l’enchaînement des sections :
> - **Première ligne** = Section d’apprentissage 1  
> - **Deuxième ligne** = Section d’apprentissage 2  
> - etc.  
> Le code (ex. `C3`) est **un identifiant interne** : ce n’est **pas lui** qui détermine l’ordre, mais **sa position dans la liste**.

---

## 📦 Bloc YAML final à transmettre

```yaml
# Attention : l’ordre des compétences ci-dessous détermine l’ordre des sections d’apprentissage.
# Ce n’est pas le code Cx qui compte, mais sa position dans la liste :
# - La première ligne correspondra à la section d’apprentissage 1
# - La deuxième ligne à la section d’apprentissage 2
# - Etc.
# Le code (C1, C2...) est conservé à des fins de traçabilité.
ordre_competences:
  - code: C1
    formulation: "[formulation compétence 1]"
    justification: "[...]"
  - code: C3
    formulation: "[formulation compétence 3]"
    justification: "[...]"
  - code: C2
    formulation: "[formulation compétence 2]"
    justification: "[...]"
  - code: C4
    formulation: "[formulation compétence 4]"
    justification: "[...]"
```









