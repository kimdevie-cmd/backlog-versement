# 🧾 Backlog – Versement Libre (VL)
> Structure par étape, avec variantes fonctionnelles par sous-branche  
> Couleur = type de variante : 🔵 Nominal | 🟣 Contrat | 🟠 B2B | 🟢 B2C | 🟡 Mix

---


## ▶️ Étape : Amount (Montant)

🔵 Nominal  
- Saisie simple du montant

🟢 B2C  
- Contrôle de saisie : montant minimum et maximum

🟠 B2B  
- Contrôle sur le plafond maximum uniquement

🟣 Contrat PERIN (B2B)  
- Saisie de l’âge de la retraite  
- Part déductible (optionnelle)

🟠 B2B + campagne de frais  
- Affichage d’un warning si campagne active

🟡 DVER / MVER  
- Affichage d’un point d’info sur la programmation

🔵 Tous (VL / DVER / MVER)  
- Saisie de l’IBAN  
- Origine des fonds obligatoire  
- Warning si montant > solde

---

## ▶️ Étape : KYC

🔵 Tous  
- Warning si clic "Suivant" sans info obligatoire

🟢 B2C  
- Alerte selon réponses incohérentes (statut, résidence fiscale…)

🟠 B2B  
- Alerte sur données client incomplètes ou incohérentes

---

## ▶️ Étape : Projet d’investissement

🟢 B2C  
- Saisie du projet d’investissement (objectif client)

⚪ B2B  
- Étape non affichée

---

## ▶️ Étape : Allocation

🟢 B2C – Gestion libre  
- Choix entre :
  - Répartition clé en main  
  - Personnalisée  
  - Libre

🟣 Contrat mandaté  
- Répartition conseillée visible  
- Répartition libre si refus du devoir de conseil

🟣 Contrat profilé / piloté  
- Répartition imposée par le contrat

🟠 B2B  
- Répartition libre sans recommandation

🔵 Tous – Répartition libre  
- Warning si montant réparti ≠ montant à investir

---

## ▶️ Étape : Frais

🟠 B2B  
- Saisie des frais dérogatoires  
- Affichage d’un warning si saisie incohérente

⚪ B2C  
- Étape non visible

---

## ▶️ Étape : Synthèse

🟣 Contrat PERIN (B2B)  
- Affichage du composant spécifique PERIN

🟣 DVER / MVER  
- Composant "Versement Programmé" visible

🟢 B2C  
- Bloc ESG visible

⚪ B2B (hors PERIN)  
- Composants spécifiques non affichés

