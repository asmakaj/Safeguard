# 🦺 SAFEGUARD AI — Sécurité intelligente pour chantiers autoroutiers

> Système innovant développé en 24 h lors d'un hackathon pour sécuriser les ouvriers sur chantiers de nuit, combinant un boîtier intelligent, un bracelet électronique et un site web de démonstration fonctionnelle.

---

## 🏆 Contexte — Hackathon 24h

Ce projet a été conçu et réalisé **from scratch en 24 heures** dans le cadre d'un hackathon sur la thématique de la sécurité des chantiers autoroutiers.

**L'équipe :**
- 2 profils informatiques
- 2 profils en génie civil

---

## 🎯 Le problème

Les chantiers autoroutiers de nuit sont des environnements à très haut risque : visibilité nulle, engins lourds en mouvement, ouvriers à pied dans des zones étroites. Les accidents par écrasement ou collision restent trop fréquents.

**SAFEGUARD AI** répond à ce défi avec un système autonome embarqué capable de détecter les situations de danger en temps réel et d'alerter instantanément — même sous la pluie, dans l'obscurité totale, ou lorsqu'un ouvrier est caché derrière un engin.

---

## 🚀 La solution en 3 composants

### 1. 📦 Boîtier intelligent — SGA-X1
Fixé sur chaque engin lourd, il embarque une suite complète de capteurs et un processeur IA :

| Capteur | Rôle | Portée |
|---|---|---|
| **LiDAR 360°** | Cartographie 3D temps réel, fonctionne dans le noir total | 100 m |
| **Radar courte portée** | Traverse pluie, brouillard, fumée (effet Doppler) | 200 m |
| **Caméra infrarouge** | Vision thermique nocturne, anonyme (formes géométriques — 100% RGPD) | — |
| **NVIDIA Jetson Orin Nano** | Fusion capteurs, calcul trajectoire & Time To Collision en **< 200 ms**, 100% local | — |

### 2. ⌚ Bracelet électronique — BRC-02
Porté par chaque ouvrier, il combine localisation ultra-précise et alertes multisensorielles :
- **UWB (Ultra Wide Band)** : localisation ±10 cm, traverse métal et béton
- **Vibration haptique** forte en cas d'alerte
- **Écran OLED directionnel** : indique la direction du danger
- **LED couleur** : vert / orange / rouge
- **Capteur cardiaque** : données transmises au rapport final
- **Autonomie 12h**

### 3. 🖥️ Application tablette — Chef de chantier
- Vue 3D temps réel de tous les engins et ouvriers
- Alertes couleur progressives (vert → orange → rouge)
- Rapport automatique généré en fin de nuit, envoyé **exclusivement au chef de chantier**

---

## ⚡ Fonctionnement — 4 étapes en < 200ms

```
T = 0 ms    →  LiDAR + UWB détectent une situation dangereuse
T = 100 ms  →  L'IA calcule la trajectoire — danger confirmé
T = 200 ms  →  Bracelet vibre + OLED + notification tablette chef de chantier
T = 2 sec   →  Alerte maximale — tous systèmes actifs
```

---

## 🎮 Démo interactive

Le site web contient une démonstration **entièrement fonctionnelle** avec 3 scénarios simulés :

| Scénario | Description |
|---|---|
| 🟢 **État normal** | Chantier sécurisé — tous connectés |
| 🟠 **Scénario 1** | Ouvrier qui entre en zone de danger (alerte Niveau 1) |
| 🔴 **Scénario 2** | Collision imminente — alerte maximale tous systèmes |
| 🔵 **Scénario 3** | Ouvrier caché derrière un engin — LiDAR aveugle, UWB prend le relais |

La démo inclut une simulation de carte de chantier temps réel, un mock de téléphone avec notifications push, et une chronologie d'alerte animée.

---

## 📊 Rapport automatique fin de nuit

Chaque nuit, le boîtier SGA-X1 génère automatiquement un rapport envoyé au chef de chantier, incluant :
- Nombre d'incidents et d'alertes déclenchées
- Captures horodatées avec coordonnées GPS de chaque incident
- Données de fréquence cardiaque des ouvriers au moment de l'alerte
- Reconstruction 3D (LiDAR + UWB) de chaque incident
- Signature numérique certifiée

---

## 🛠️ Stack technique (démo web)

- **HTML5 / CSS3 / JavaScript** — site de démo mono-fichier, aucune dépendance
- **Google Fonts** — Barlow Condensed pour l'identité visuelle
- Animations CSS natives, QR code généré par canvas, simulation d'alertes en temps réel

---

## 📁 Contenu du dépôt

```
├── safeguard_final.html   # Site web de démonstration complet (mono-fichier)
└── README.md              # Ce fichier
```

> **Note :** Le fichier `incident_3d.mp4` (reconstruction 3D des incidents) est référencé dans la démo mais non inclus dans ce dépôt.

---

## 📋 Caractéristiques clés

- ✅ **Installation en 20 min** sur tout engin existant
- ✅ **100% local** — aucun cloud, aucun réseau requis sur chantier
- ✅ **IP67** — résistant aux intempéries
- ✅ **Nuit & jour** — multi-capteurs complémentaires
- ✅ **100% RGPD** — aucune capture de visage, anonymat garanti
- ✅ **< 200ms** temps de réaction de bout en bout


---

*SAFEGUARD AI — SGA-X1 · BRC-02 · Hackathon 2026*
