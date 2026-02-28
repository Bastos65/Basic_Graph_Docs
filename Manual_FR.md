# BASIC GRAPH - Documentation Complète

> ⚠️ **AVERTISSEMENT** : Ce dépôt contient uniquement la documentation utilisateur. Aucun code source, algorithme, logique serveur ou mécanisme de licence n'est inclus. Toute tentative de rétro-ingénierie du produit est interdite.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Platform](https://img.shields.io/badge/platform-Garmin%20Connect%20IQ-green)
![API](https://img.shields.io/badge/API-5.0.0%2B-orange)

---

## Table des Matières

1. [Vue d'ensemble](#vue-densemble)
2. [Fonctionnalités Principales](#fonctionnalités-principales)
3. [Interface Utilisateur](#interface-utilisateur)
4. [Configuration](#configuration)
   - [Paramètres Système](#paramètres-système)
   - [Paramètres d'Affichage](#paramètres-daffichage)
   - [Champs de Données](#champs-de-données)
   - [Champ Graphique](#champ-graphique)
   - [Personnalisation des Couleurs](#personnalisation-des-couleurs)
   - [Météo](#météo)
5. [Types de Données Disponibles](#types-de-données-disponibles)
6. [Glossaire](#glossaire)
7. [Annexes](#annexes)

---

![BASIC GRAPH Banner](docs/images/Banner.jpg)

---

## Vue d'ensemble

**BASIC GRAPH** est un cadran de montre épuré et riche en données pour les montres Garmin Connect IQ. Construit autour d'un champ graphique central affichant des données historiques, il combine 6 champs circulaires, des champs classiques supérieurs et une personnalisation étendue pour fournir un maximum d'informations en un coup d'œil.

### Caractéristiques Clés

- 📊 **Champ Graphique Central** : Graphique en ligne ou en barres avec jusqu'à 4 heures d'historique
- 🔵 **6 Champs Circulaires** : Positionnés à 1h, 3h, 5h, 7h, 9h, 11h
- 📋 **3 Champs Classiques Supérieurs** : Gauche, Centre, Droite configurables
- 🎨 **22 Couleurs Personnalisables** : Contrôle complet des couleurs
- 🌦️ **Intégration Météo** : Garmin Weather et OpenWeatherMap
- ⚡ **Optimisation Batterie** : Modes économie d'énergie intelligents
- 🌍 **Support Multilingue** : 19 langues disponibles
- 🎯 **Anneau d'Objectif** : Suivi visuel de progression des objectifs

---

## Fonctionnalités Principales

### 1. Affichage de l'Heure

- Format 12h ou 24h
- Affichage des secondes (3 modes : Caché, Normal, Toujours Actif)
- Zéro de tête optionnel pour les heures
- Support AM/PM en format 12h
- Couleurs indépendantes pour les heures, minutes, secondes, séparateur

### 2. Champ Graphique

La fonctionnalité centrale de BASIC GRAPH — un graphique configurable affichant des données en série temporelle :

- **Graphique en Ligne** : Représentation en courbe
- **Graphique en Barres** : Représentation en barres verticales
- **Durée** : 1 à 4 heures d'historique (pour les données non-7-jours)
- **Mode 7 Jours** : Affiche l'historique sur 7 jours avec lettres des jours optionnelles
- **Ligne d'objectif** : Affichage optionnel de la valeur objectif
- **Objectif personnalisé** : Remplacer l'objectif système par une valeur personnalisée

### 3. Champs Circulaires de Données

Six champs circulaires positionnés aux positions d'horloge 1h, 3h, 5h, 7h, 9h, 11h :

- Affichage de valeur
- Titre personnalisable
- Affichage de l'unité
- Plusieurs modes d'affichage
- Configuration de couleur indépendante

### 4. Champs Classiques Supérieurs

Trois champs de données en haut du cadran :

- Champ Supérieur Gauche
- Champ Supérieur Centre
- Champ Supérieur Droit
- Icônes colorées (jeu plein ou contour)
- Valeurs textuelles

### 5. Champ Texte Supérieur

- Type de données entièrement configurable
- Plusieurs modes d'affichage (valeur, titre+valeur, objectif, etc.)
- Titre personnalisable

### 6. Indicateurs Info

Quatre indicateurs visuels :

1. **Info 1** : Indicateur configurable
2. **Info 2** : Indicateur configurable
3. **Info 3** : Indicateur configurable
4. **Info 4** : Indicateur configurable

### 7. Anneau d'Objectif

- Visualisation graphique de la progression
- Plusieurs types de données d'objectif
- Plage configurable (min/max)

### 8. Date

- 7 formats d'affichage
- Jour de la semaine
- Support de format international

### 9. Météo

- **Sources** : Garmin Weather et/ou OpenWeatherMap
- **Données Disponibles** :
  - Température actuelle, ressentie, min/max
  - Description et icône météo
  - Humidité
  - Vitesse et direction du vent
  - Pression atmosphérique (OWM)
  - Couverture nuageuse (OWM)
  - Visibilité (OWM)
  - Probabilité de précipitations (GW)

---

## Interface Utilisateur

### Structure de l'Écran

![Disposition du Cadran](docs/images/Display_Overview.png)

*Disposition BASIC GRAPH affichant toutes les zones configurables*

### Légende
- **Heure** : Affichage de l'heure
- **Date** : Affichage de la date
- **Graphique** : Champ graphique central
- **Circ 1h/3h/5h/7h/9h/11h** : Champs circulaires
- **SG/SC/SD** : Champs supérieurs (Gauche/Centre/Droit)
- **I1/I2/I3/I4** : Indicateurs d'information
- **Anneau Objectif** : Anneau de progression d'objectif

---

## Configuration

### Paramètres Système

#### Taux de Rafraîchissement des Données
Contrôle la fréquence de mise à jour des données :

- **Rafraîchissement Complet** : Mise à jour complète chaque seconde (consommation maximale)
- **Taux Élevé** : Rafraîchissement élevé
- **Taux Moyen** : Rafraîchissement moyen (recommandé)
- **Taux Faible** : Rafraîchissement faible (économie de batterie)

#### Économie d'Énergie

**Délai Veille Écran** : Délai en minutes avant l'activation de l'économiseur d'écran (-1 pour désactiver)

**Délai Extinction Écran** : Délai en minutes avant l'extinction de l'écran (-1 pour désactiver)

#### Widget

**Lancer Widget Appui Long** : Lancer le widget sur appui long (écran tactile uniquement)

---

### Paramètres d'Affichage

#### Format de l'Heure

**Utiliser le Format Militaire** :
- `true` : Format 24 heures
- `false` : Format 12 heures (AM/PM)

**Zéro de Tête des Heures** :
- `true` : Afficher le zéro de tête (01, 02, 03...)
- `false` : Sans zéro de tête (1, 2, 3...)

**Mode d'Affichage des Secondes** :
1. **Caché** : Secondes masquées
2. **Normal** : Affichage normal des secondes
3. **Toujours Actif** : Toujours affiché

#### Format de Date

7 modes d'affichage disponibles :

1. `[JJ jj Mois]` : Lun 15 Janvier
2. `[JJ jj/mm]` : Lun 15/01
3. `[jj/mm/aaaa]` : 15/01/2026
4. `[JJ Mois jj]` : Lun Janvier 15
5. `[Mois jj JJ]` : Janvier 15 Lun
6. `[JJ mm/jj]` : Lun 01/15
7. `[aaaa/mm/jj]` : 2026/01/15

---

### Champs de Données

#### Configuration de Chaque Champ

Pour chaque champ de données, vous pouvez configurer :

1. **Type de Données** : Choisir parmi 73+ types (voir section Types de Données)
2. **Titre Personnalisé** : Texte libre pour remplacer le titre par défaut
3. **Mode d'Affichage** : Comment afficher les données

#### Modes d'Affichage

##### Champs Circulaires (1h, 3h, 5h, 7h, 9h, 11h)

0. **Valeur** : Valeur uniquement
1. **Titre + Valeur** : Titre au-dessus de la valeur
2. **Valeur + Unité** : Valeur avec unité
3. **Valeur + Titre** : Valeur avec titre en dessous
4. **Titre Valeur Unité** : Titre, valeur, unité

##### Champ Texte Supérieur

0. **Valeur** : Valeur uniquement
1. **Titre + Valeur** : Titre et valeur
2. **Valeur + Unité** : Valeur avec unité
3. **Valeur + Titre** : Valeur avec titre
4. **Titre Valeur Unité** : Titre, valeur, unité
5. **Titre** : Titre uniquement
6. **Objectif** : Affichage de l'objectif
7. **Valeur / Objectif** : Valeur sur objectif
8. **Pourcentage Objectif** : Pourcentage de l'objectif
9. **Restant** : Restant pour atteindre l'objectif

---

### Champ Graphique

Le champ graphique est l'élément central de BASIC GRAPH.

#### Type de Données du Graphique

Sélectionner le type de données à afficher dans le graphique parmi tous les types disponibles.

#### Mode d'Affichage du Graphique

- **Graphique en Ligne** : Courbe continue
- **Graphique en Barres** : Barres verticales

#### Durée du Graphique

Pour les types de données non-7-jours : durée en heures (1 à 4 heures).

#### Options 7 Jours

- **Afficher les Lettres des Jours** : Afficher les abréviations des jours sous les barres
- **Afficher l'Objectif du Graphique** : Afficher une ligne horizontale d'objectif

#### Configuration de l'Objectif

- **Afficher l'Objectif du Graphique** : Activer/désactiver la ligne d'objectif
- **Objectif Personnalisé du Graphique** : Remplacer la valeur de l'objectif système (0 = utiliser l'objectif système)

---

### Personnalisation des Couleurs

BASIC GRAPH propose **22 couleurs personnalisables** :

| ID | Élément |
|----|---------|
| 0 | Couleur de Fond |
| 1 | Couleur des Lignes de Séparation |
| 2 | Couleur Titre/Unité des Champs Circulaires |
| 3 | Couleur Valeur des Champs Circulaires |
| 4 | Couleur Texte des Champs Texte |
| 5 | Couleur Valeur des Champs de Données |
| 6 | Couleur Titre/Icône Champ Supérieur Gauche |
| 7 | Couleur Titre/Icône Champ Supérieur Centre |
| 8 | Couleur Titre/Icône Champ Supérieur Droit |
| 9 | Couleur des Heures |
| 10 | Couleur du Séparateur Heure |
| 11 | Couleur des Minutes |
| 12 | Couleur des Secondes & AM/PM |
| 13 | Couleur Valeur du Graphique |
| 14 | Couleur Objectif du Graphique |
| 15 | Couleur Info Inactif |
| 16 | Couleur Info 1 Actif |
| 17 | Couleur Info 2 Actif |
| 18 | Couleur Info 3 Actif |
| 19 | Couleur Info 4 Actif |
| 20 | Couleur Anneau Objectif Inactif |
| 21 | Couleur Anneau Objectif Actif |

### Palette de Couleurs Prédéfinie

Le cadran propose **67 couleurs prédéfinies** organisées par famille.

➡️ **[Voir la liste complète des couleurs](https://pay.b65dev.com/portfolio/faqs#faq-colors)**

### Options de Couleurs Spéciales

**Couleur Adaptative Batterie** : Adapte automatiquement la couleur selon le niveau de batterie

**Icônes Météo Colorées** : Colorie les icônes météo selon les conditions

**Couleurs Personnalisées** : Définir jusqu'à 3 couleurs personnalisées via code hexadécimal (format : `0xffffff` ou `ffffff`)

---

### Météo

#### Configuration du Fournisseur

**Fournisseur Météo** : Sélection du service météo

1. **Garmin Weather (GW)** : Service natif Garmin
2. **OpenWeatherMap (OWM)** : Service externe nécessitant une clé API
3. **Garmin Weather + OpenWeatherMap** : Priorité Garmin, complément OWM
4. **OpenWeatherMap + Garmin Weather** : Priorité OWM, complément Garmin

#### OpenWeatherMap

**Clé Météo** : Clé API OpenWeatherMap (32 caractères max)

Pour obtenir une clé API :
1. Créer un compte sur [openweathermap.org](https://openweathermap.org)
2. Générer une clé API gratuite
3. Copier la clé dans les paramètres

**Appel Météo** : Affiche l'heure du dernier appel API (lecture seule)

---

### Unités de Mesure

#### Altitude
- Mètres (m)
- Pieds (ft)

#### Distance
- Kilomètres (km)
- Miles (mi)
- Miles Nautiques Internationaux (nm)

#### Température
- Celsius (°C)
- Fahrenheit (°F)
- Kelvin (°K)

**Décalage Température** : Correction du capteur de température (valeur numérique)

#### Pression
- Hectopascal (hPa)
- Millimètres de Mercure 0°C (mmHg)
- Pouce de Mercure 0°C (inHg)

#### Poids
- Kilogrammes (kg)
- Livres (lbs)

#### Vitesse du Vent
- Mètres / Secondes (m/s)
- Kilomètres / Heures (km/h)
- Miles / Heures (mi/h)
- Nœuds (kn)
- Échelle Beaufort (bf)

#### Direction du Vent
- **Direction en Degrés** : Affichage en degrés (000-360)
- **Direction Cardinale** : Affichage cardinal (N, NE, E, SE, S, SO, O, NO)

---

### Paramètres Avancés

#### Textes Personnalisés

**Valeur Texte Personnalisé 1** : Texte libre pour affichage personnalisé  
**Valeur Texte Personnalisé 2** : Second texte libre

#### Compte à Rebours

**Jour Cible du Compte à Rebours** : Date cible du compte à rebours  
**Heure Cible du Compte à Rebours** : Heure cible (format HH:mm:ss, ex. : 14:30:00)

#### Fuseaux Horaires

Configuration de 4 fuseaux horaires supplémentaires :

- **Fuseau Horaire 2** : Format UTC (ex. : +02:00 ou -05:30)
- **Fuseau Horaire 3** : Format UTC
- **Fuseau Horaire 4** : Format UTC
- **Fuseau Horaire 5** : Format UTC

Format : HH:mm avec signe + ou - (ex. : `+02:00`, `-05:30`)

#### Jeux d'Icônes

**Jeu d'Icônes** :
- **Icônes Pleines** : Icônes solides
- **Icônes Contour** : Icônes avec contour

---

## Types de Données Disponibles

BASIC GRAPH supporte **73+ types de données différents**. Voici la liste complète :

### Activité Physique

| Type | Description |
|------|-------------|
| Minutes Actives : Quotidien | Minutes actives quotidiennes |
| Minutes Actives : Hebdomadaire | Minutes actives hebdomadaires |
| Calories : Brûlées Quotidien | Calories brûlées quotidiennes |
| Calories : Brûlées Actives Quotidien | Calories actives brûlées |
| Pas Quotidiens | Nombre de pas quotidiens |
| Distance : Quotidienne | Distance du jour |
| Distance : Hebdomadaire | Distance de cette semaine |
| Étages Montés : Quotidien | Étages montés aujourd'hui (si disponible) |

### Distances Spécifiques

| Type | Description |
|------|-------------|
| Distance Vélo : Semaine | Distance cyclisme de la semaine |
| Distance Vélo : 30 Jours | Distance cyclisme sur 30 jours |
| Distance Vélo : Mois en cours | Distance cyclisme du mois en cours |
| Distance Course : Semaine | Distance course à pied de la semaine |
| Distance Course : 30 Jours | Distance course sur 30 jours |
| Distance Course : Mois en cours | Distance course du mois en cours |
| Poussées | Nombre de poussées (si disponible) |
| Distance Poussées Quotidienne | Distance poussées quotidienne (si disponible) |

### Santé et Bien-être

| Type | Description |
|------|-------------|
| Fréquence Cardiaque | Fréquence cardiaque actuelle |
| FC Min/Max (4 Heures) | FC min/max sur 4 heures |
| Body Battery | Niveau de body battery (si disponible) |
| Niveau de Stress | Niveau de stress (si disponible) |
| Fréquence Respiratoire | Fréquence respiratoire (si disponible) |
| Saturation en Oxygène | SpO2 (si disponible) |
| Temps de Récupération | Temps de récupération hh:mm (si disponible) |
| Poids | Poids en kg |

### Performance Sportive

| Type | Description |
|------|-------------|
| VO2 Max Cyclisme | VO2 Max cyclisme (si disponible) |
| VO2 Max Course | VO2 Max course à pied (si disponible) |
| Prédicteur Course 5K | Prédiction temps 5K |
| Prédicteur Course 10K | Prédiction temps 10K |
| Prédicteur Semi-Marathon | Prédiction semi-marathon |
| Prédicteur Marathon | Prédiction marathon |
| Statut d'Entraînement | Statut d'entraînement |

### Système et Batterie

| Type | Description |
|------|-------------|
| Batterie en Jours | Autonomie batterie en jours |
| Batterie en Pourcents | Niveau batterie en % |
| Intensité Solaire | Intensité solaire (si disponible) |
| Téléphone Connecté | Téléphone connecté |
| Nombre d'Alarmes | Nombre d'alarmes |
| Nombre de Notifications | Nombre de notifications |
| Niveau Alerte Mouvement | Niveau d'alerte inactivité |
| Ne Pas Déranger Activé | Mode ne pas déranger activé |

### Environnement

| Type | Description |
|------|-------------|
| Altitude | Altitude actuelle (si disponible) |
| Pression du Capteur | Pression atmosphérique (si disponible) |
| Température du Capteur | Température du capteur (si disponible) |

### Météo (Garmin Weather)

| Type | Description |
|------|-------------|
| Description Météo | Description météo |
| Température Météo | Température météo |
| Température Ressentie | Température ressentie |
| Température Min / Max | Températures min/max (GW uniquement) |
| Humidité | Humidité |
| Probabilité de Précipitations | Probabilité de précipitations (GW) |
| Vitesse/Direction du Vent | Vitesse et direction du vent |
| Heure MàJ Garmin Weather | Heure de mise à jour Garmin Weather |

### Météo (OpenWeatherMap)

| Type | Description |
|------|-------------|
| Station Météo | Station météo (OWM uniquement) |
| Couverture Nuageuse | Couverture nuageuse (OWM uniquement) |
| Pression Météo | Pression (OWM uniquement) |
| Visibilité Météo | Visibilité (OWM uniquement) |
| Heure MàJ OWM | Heure de mise à jour OpenWeatherMap |

### Soleil et Lune

| Type | Description |
|------|-------------|
| Lever du Soleil | Lever du soleil |
| Coucher du Soleil | Coucher du soleil |
| Prochain Événement Solaire | Prochain événement solaire |
| Aube Civile | Aube civile |
| Crépuscule Civil | Crépuscule civil |
| Âge de la Lune | Âge de la lune |
| Illumination Lunaire | Illumination lunaire |
| Phase Lunaire | Phase lunaire |

### Date et Heure

| Type | Description |
|------|-------------|
| Date | Date actuelle |
| Jour de l'Année | Jour de l'année |
| Semaine de l'Année | Semaine de l'année |
| Fuseau Horaire 2 | Fuseau horaire 2 |
| Fuseau Horaire 3 | Fuseau horaire 3 |
| Fuseau Horaire 4 | Fuseau horaire 4 |
| Fuseau Horaire 5 | Fuseau horaire 5 |
| Compte à Rebours | Compte à rebours |

### Personnalisation

| Type | Description |
|------|-------------|
| Texte Personnalisé | Texte personnalisé 1 |
| Texte Personnalisé 2 | Texte personnalisé 2 |
| Champ Caché | Champ caché |

### Debug

| Type | Description |
|------|-------------|
| Données Debug | Données de débogage |

---

## Glossaire

- **AMOLED** : Type d'écran à diodes électroluminescentes organiques à matrice active
- **API** : Interface de programmation d'application
- **Connect IQ** : Plateforme Garmin pour applications tierces
- **GW** : Garmin Weather (service météo Garmin)
- **OWM** : OpenWeatherMap (service météo externe)
- **SpO2** : Saturation pulsée en oxygène
- **VO2 Max** : Consommation maximale d'oxygène
- **UTC** : Temps Universel Coordonné

---

## Annexes

### Formats des Paramètres

#### Couleurs Personnalisées
Format hexadécimal : `0xRRGGBB` ou `RRGGBB`
- RR = Rouge (00-FF)
- GG = Vert (00-FF)
- BB = Bleu (00-FF)

Exemple : `0xFF0000` = Rouge pur

#### Fuseaux Horaires
Format : `±HH:mm`
- Signe + pour l'Est, - pour l'Ouest
- HH = Heures (00-14)
- mm = Minutes (00 ou 30)

Exemples :
- `+01:00` = UTC+1 (Paris)
- `-05:00` = UTC-5 (New York)
- `+05:30` = UTC+5:30 (Inde)

#### Heure Compte à Rebours
Format : `HH:mm:ss`
- HH = Heures (00-23)
- mm = Minutes (00-59)
- ss = Secondes (00-59)

Exemple : `14:30:00` = 14h30

### Codes des Phases Lunaires

Les phases lunaires sont numérotées de 0 à 7 :
- 0 : Nouvelle Lune
- 1 : Premier Croissant
- 2 : Premier Quartier
- 3 : Lune Gibbeuse Croissante
- 4 : Pleine Lune
- 5 : Lune Gibbeuse Décroissante
- 6 : Dernier Quartier
- 7 : Dernier Croissant

---

**Dernière mise à jour** : 28 Février 2026  
**Version du document** : 1.0  
**Auteur** : Bastos65

---

*Ce document est fourni "tel quel" sans garantie d'aucune sorte. Le développeur se réserve le droit de modifier les fonctionnalités et la documentation sans préavis.*
