# SPEC-PMSI
Spécificités techniques et fonctionnelles PMSI TdocT
# PMSI+IA API - CodeIgniter

Cette API REST permet de connecter le logiciel de codage PMSI intelligent à des systèmes tiers (Mediboard, Shaker, ApiCrypt, etc.)

## 🔌 Fonctionnalités principales

- Analyse IA des dossiers (Shaker Symptômes, Comprehend)
- Codage CIM-10 / CCAM / NABM
- Connexion Mediboard et autres SIH
- Communication avec les équipes soignantes
- Tableau de bord patient intelligent

## 🚀 Endpoints REST disponibles

| Méthode | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/login` | Authentification par JWT |
| GET | `/api/patients` | Liste des patients |
| POST | `/api/patient/{id}/analyse` | Analyse IA |
| GET | `/api/patient/{id}/codes` | Récupération des codes |
| POST | `/api/shaker/analyse` | Analyse shaker |
| POST | `/api/mediboard/sync` | Sync vers Mediboard |

## 🔐 Sécurité

- Authentification par JWT (`Authorization: Bearer <token>`)
- Filtre `AuthTokenFilter` appliqué à tous les endpoints `/api/*`

## 🧱 Technologies

- CodeIgniter 4
- Firebase JWT
- Shaker API
- Mediboard API
- Base MySQL ou PostgreSQL

## 🧪 Tests & Déploiement

- Compatible Postman / Insomnia
- Utilisable en frontal avec React/Vue ou application mobile
- Dockerisable facilement

---

> Pour toute contribution : créer une branche `feature/nom-fonction` puis PR vers `main`
