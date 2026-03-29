https://github.com/chaymaaelmouini-droid/Chaymaa-el-mouini-IG-project/blob/main/WhatsApp%20Image%202026-03-29%20at%2000.30.35.jpeg

# ☕ Compte Rendu — Analyse des Ventes Coffee Sales

**Préparé par : CHAYMAA EL MOUINI**
*ENCG Settat — Université Hassan 1er*
*Performance Commerciale | Mars 2024 → Mars 2025*

---

## 1. Contexte & Objectifs

Ce compte rendu présente une analyse complète des données de ventes d'un établissement de café sur une période de 13 mois (mars 2024 à mars 2025). L'objectif est d'identifier les tendances de consommation, les produits les plus performants, les pics d'activité temporels et les leviers d'optimisation commerciale.

**Source des données :** `Coffe_Sales_Data.xlsx` — 3 547 transactions, feuille `Coffe_sales`
**Outils utilisés :** Python (pandas), Excel (openpyxl), Dashboard HTML (Chart.js)

---

## 2. Indicateurs Clés de Performance (KPI)

| Indicateur | Valeur |
|---|---|
| **Chiffre d'Affaires Total** | 112 246 € |
| **Nombre de Transactions** | 3 547 |
| **Panier Moyen** | 31,65 € |
| **Top Produit (CA)** | Latte — 26 875 € |
| **Meilleur Mois** | Mars 2024 — 15 892 € |
| **Pic Horaire** | 10h00 — 10 199 € cumulés |
| **Mode de Paiement** | 100 % carte bancaire |

---

## 3. Analyse des Ventes par Produit

### 3.1 Classement par Chiffre d'Affaires

| Rang | Produit | Ventes | CA (€) | Prix Moy. (€) | Part CA |
|:---:|---|:---:|---:|:---:|:---:|
| 🥇 | Latte | 757 | 26 875 | 35,50 | 23,9 % |
| 🥈 | Americano with Milk | 809 | 24 751 | 30,60 | 22,0 % |
| 🥉 | Cappuccino | 486 | 17 439 | 35,88 | 15,5 % |
| 4 | Americano | 564 | 14 650 | 25,98 | 13,0 % |
| 5 | Hot Chocolate | 276 | 9 933 | 35,99 | 8,8 % |
| 6 | Cocoa | 239 | 8 521 | 35,65 | 7,6 % |
| 7 | Cortado | 287 | 7 385 | 25,73 | 6,6 % |
| 8 | Espresso | 129 | 2 690 | 20,85 | 2,4 % |

### 3.2 Observations

- Le **Latte** et l'**Americano with Milk** représentent à eux seuls **45,9 %** du chiffre d'affaires total.
- L'**Americano with Milk** est le produit le plus vendu en volume (809 unités) mais deuxième en CA, ce qui s'explique par un prix moyen inférieur au Latte.
- L'**Espresso** est le produit le moins performant, tant en volume qu'en CA, avec seulement 129 ventes et un prix moyen de 20,85 €.
- Les produits à base de lait chaud (Latte, Cappuccino, Hot Chocolate, Cocoa) concentrent **55,8 %** du CA total.

---

## 4. Analyse Temporelle

### 4.1 Évolution Mensuelle du CA

| Mois | Transactions | CA (€) | Part CA |
|---|:---:|---:|:---:|
| Janvier | 201 | 6 399 | 5,7 % |
| Février | 423 | 13 215 | 11,8 % |
| **Mars** | **494** | **15 892** | **14,2 %** |
| Avril | 168 | 5 720 | 5,1 % |
| Mai | 241 | 8 164 | 7,3 % |
| Juin | 223 | 7 618 | 6,8 % |
| Juillet | 237 | 6 916 | 6,2 % |
| Août | 272 | 7 614 | 6,8 % |
| Septembre | 344 | 9 989 | 8,9 % |
| **Octobre** | **426** | **13 891** | **12,4 %** |
| Novembre | 259 | 8 591 | 7,7 % |
| Décembre | 259 | 8 238 | 7,3 % |

**Observations :**
- Deux pics majeurs sont identifiés : **mars** (début de printemps) et **octobre** (rentrée/automne), correspondant probablement à des périodes d'affluence scolaire ou universitaire.
- Le mois d'**avril** enregistre la performance la plus faible (5 720 €, 168 transactions), soit une chute de -64 % par rapport à mars — creux potentiellement lié aux vacances.
- La seconde moitié de l'année (sept.–déc.) est globalement plus stable que la première moitié.

### 4.2 Performance par Jour de la Semaine

| Jour | Transactions | CA (€) |
|---|:---:|---:|
| **Mardi** | 572 | **18 168 €** |
| **Lundi** | 544 | 17 363 € |
| Vendredi | 531 | 16 803 € |
| Jeudi | 510 | 16 091 € |
| Mercredi | 500 | 15 750 € |
| Samedi | 465 | 14 734 € |
| Dimanche | 425 | 13 336 € |

**Observations :**
- Le **mardi** est le jour le plus rentable, tandis que le **dimanche** affiche le CA le plus faible.
- La semaine de travail (lundi–vendredi) génère **75,5 %** du CA total, contre 24,5 % pour le week-end.
- L'écart entre le meilleur jour (mardi, 18 168 €) et le pire (dimanche, 13 336 €) est de **+36 %**.

### 4.3 Distribution Horaire

| Tranche | CA Cumulé (€) | Pic ? |
|---|---:|:---:|
| 6h – 8h | 10 013 | |
| 9h – 11h | **25 916** | ⭐ Matin |
| 12h – 14h | 21 622 | |
| 15h – 17h | **24 168** | ⭐ Après-midi |
| 18h – 22h | 30 526 | |

- Le **pic principal** se situe à **10h00** (10 199 € de CA cumulé sur la période).
- La tranche **16h00** est le second pic important (9 032 €), correspondant à la pause de l'après-midi.
- L'activité reste soutenue jusqu'à **22h00**, suggérant une clientèle nocturne non négligeable.

---

## 5. Profil de la Clientèle

- **Mode de paiement exclusif :** 100 % des transactions sont réglées par carte bancaire — aucune transaction en espèces n'est enregistrée.
- **Répartition temporelle équilibrée :** matin (33,3 %), après-midi (34,0 %) et soir (32,7 %) — la clientèle est répartie de manière homogène sur la journée.
- **Panier moyen stable :** à 31,65 €, le panier moyen varie peu selon les périodes, traduisant une offre à tarification cohérente.

---

## 6. Points Forts & Points de Vigilance

### ✅ Points Forts

- **Diversité de l'offre** : 8 produits couvrant différents segments (cafés, chocolats, boissons chaudes).
- **Régularité** : présence active sur l'ensemble des plages horaires (6h–22h), 7j/7.
- **Produits stars** solides : Latte et Americano with Milk assurent une base de CA stable.
- **Mois de mars** exceptionnel : meilleure performance de la période avec 494 transactions.

### ⚠️ Points de Vigilance

- **Dépendance aux 2 produits leaders** : Latte + Americano with Milk = 45,9 % du CA. Une baisse de leur popularité impacterait fortement les revenus.
- **Creux d'avril** : la chute brutale en avril (-64 % vs mars) mérite d'être anticipée (promotions saisonnières, offres spéciales).
- **Espresso sous-performant** : seulement 129 ventes sur 13 mois — à réévaluer (prix, visibilité, positionnement).
- **Week-end peu exploité** : le dimanche représente seulement 11,9 % du CA hebdomadaire — marge de progression possible.

---

## 7. Recommandations

1. **Valoriser les produits à forte marge** : mettre en avant le Latte et le Cappuccino (prix moyen ~35 €) plutôt que l'Americano (25 €) pour augmenter le panier moyen.

2. **Stratégie anti-creux d'avril** : lancer des offres promotionnelles ou des formules "printemps" dès fin mars pour limiter la baisse d'activité.

3. **Dynamiser le week-end** : créer des offres dédiées au samedi/dimanche (brunch, formules duo, fidélité) pour combler l'écart avec les jours de semaine.

4. **Retravailler l'Espresso** : envisager une révision du prix, une mise en avant en caisse, ou un packaging "shot express" pour les clients pressés.

5. **Capitaliser sur les pics** : renforcer les effectifs aux heures 10h et 16h, et proposer des formules "pause café" pour maximiser le CA pendant ces créneaux.

6. **Analyser le creux de janvier** : avec seulement 201 transactions, janvier est le mois le plus faible — investiguer les causes (météo, vacances, concurrence saisonnière).

---

## 8. Conclusion

Sur la période mars 2024 – mars 2025, l'établissement affiche une performance commerciale globalement solide avec **112 246 € de CA** pour **3 547 transactions**. La structure de l'offre est bien établie autour de produits phares (Latte, Americano with Milk, Cappuccino), et la clientèle est fidèle et répartie sur toute la journée.

Les principaux axes d'amélioration portent sur la **gestion des creux saisonniers** (avril, janvier), la **valorisation du week-end**, et l'**optimisation de la gamme** en repositionnant les produits à faible rotation comme l'Espresso.

---

*Rapport généré automatiquement à partir du fichier `Coffe_Sales_Data.xlsx`*
*ENCG Settat — Université Hassan 1er | Mars 2026*
