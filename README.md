# 🍫 Forecast Pâtisserie

## 🔎 Problème

Un réseau de **8 boutiques** de pâtisserie doit préparer son année N+1.

* Historique : **2 à 7 années** par boutique.
* Les plus anciennes (Carnot, Sieyès, Gambetta) : **7 ans complets**.
* Les plus récentes (Voltaire, République, Jaurès) : seulement **2 à 3 ans**.

**Enjeux :**

* Prévoir les ventes (boutique et global).
* Planifier la main-d’œuvre (pâtissiers par mois).
* Sécuriser les approvisionnements en chocolat (palettes 500 kg, stock mini 300 kg, délai 1 mois).

❌ Sans prévision fiable → ruptures, surcoûts RH, surstock immobilisé.
🎯 Objectif : transformer un **forecast** en **plan opérationnel (RH + achats)**.

---

## 🛠️ Méthode

### 1. Cycle de vie identifié

Analyse des progressions moyennes toutes boutiques :

* Année 2 = **+119 %** (hypercroissance),
* Année 3 = **+19 %**,
* Années 4–7 = **+1 à 4 %** → stabilisation/maturité.

### 2. Forecast hybride

* **Phase stabilisée (années 4–7)** : régression linéaire (`FORECAST`), contrôlée par le **R²** (≥0,8).
* **Phase hypercroissance (années 1–3) ou historique court** : application du **taux moyen réseau**.
* **Choix final** par boutique selon la qualité du modèle.

### 3. Phasing mensuel

* Ventilation du forecast annuel selon les poids historiques (ex. décembre ≈ 11,36 %).

### 4. Traduction opérationnelle

* Conversion en **kg chocolat consommé** (mix produits),
* **Heures de production** → **pâtissiers nécessaires**.

### 5. Plan MRP chocolat

* Stock initial : 380 kg – Stock mini : 300 kg – Lot : 500 kg – Délai : 1 mois.
* Règle : `Stock fin = Stock début + Livraison – Consommation`.
* Si <300 kg → commande automatique d’une palette.

---

## 📊 Résultats

* Prévision annuelle réseau (N+1) : **\~870 000 unités vendues**.
* Décembre : besoin de **14 pâtissiers** (vs 10 en capacité actuelle).
* Plan MRP chocolat : commandes calées → **zéro rupture, zéro surstock**.

---

## 🚀 Recommandation

* **Ressources humaines** : anticiper les pics, prévoir **+4 renforts** en fin d’année, lisser la production des produits stockables.
* **Supply chain** : sécuriser le chocolat (commande avant le 10, lot 500 kg), optimiser les stocks → réduire coûts et risques.
* **Pilotage** : fiabilité renforcée (R² + taux moyens réseau), KPI de prévision par boutique, rituel mensuel forecast → production → achats.


