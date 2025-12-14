# Abaque de charge – Front & Intégration (Assurance Vie)

## Objectif
Cet abaque permet d’estimer la charge de développement d’une User Story
en fonction de sa complexité fonctionnelle, UI et d’intégration.
Il est utilisé pour dimensionner le scope, alimenter la roadmap et planifier les sprints.

---

## Niveaux de complexité

| Complexité | Libellé         | Description synthétique                                                                 | Éléments inclus                                                                                  | Charge estimée (JH) |
|------------|------------------|------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|---------------------|
| S          | Simple           | Fonctionnalité élémentaire                                                               | UI légère, affichage simple, aucune ou très peu de règles métier, pas de mapping                | 1 – 2               |
| M          | Moyenne          | Fonctionnalité standard                                                                  | UI avec interactions simples (bouton, warning), 1–2 règles métier, mapping simple              | 3 – 4               |
| L          | Complexe         | Fonctionnalité riche                                                                     | UI complexe, plusieurs règles métier, dépendances de contexte, mapping structuré                | 5 – 6               |
| XL         | Très complexe    | Module avancé / structurant                                                              | UI avancée (filtres, overlay, recherche), logique métier dense, mapping complexe ou multiple    | 7 – 9+              |

---

## Règles d’application

- La **complexité est évaluée par User Story**, pas par écran complet.
- Chaque **variante d’un step** (selon contexte B2B / B2C / contrat / canal) est considérée comme **une US distincte**.
- La charge inclut :
  - Développement front
  - Règles de gestion
  - Intégration via swagger / JSON mockés
- Le KT et la montée en compétence des équipes sont considérés comme **déjà réalisés**.

---

## Exemples d’application

- **Pop-up de confirmation simple après synthèse** → `S`
- **Step avec warning conditionnel + bouton suivant** → `M`
- **Écran avec plusieurs variantes métier selon le contexte** → `L`
- **Module de recherche avec filtres, overlay et mise à jour dynamique** → `XL`

---
